
# DICTIONARY API REFERENCE
Base URL: https://api.dictionaryapi.dev/
## Overview
Retrieves dictionary information for a specified english word, including its definition, part of speech, phonetic spelling, pronunciation audio, and usage example. Useful for building vocabulary apps, language learning tools or any feature that needs word definitions on demand. No authentication key is required.
## Authentication
No key required.
## Request details 
**Method**:`` GET``   
 **URL**:  `{{baseUrl}}/api/v2/entries/{{languageCode}}/{{word}}`
### Path Parameters

|  **Name**   |  **Type**  | **Required?**  |  **Description**  | **Example** |
| ----------- | :--------- | ------------- | ----------------- | ----------- |
| languageCode| string | Yes| Code for the language in which you want the word definition. | en
| Word | string | Yes| The word you want to look up. Must be spelled correctly and be in the dictionary. | spin
## Example Request
 `` GET https://api.dictionaryapi.dev/api/v2/entries/en/spin `` 
 This requests the dictionary information available for the english word 'spin'.
## Example Response
```json 
{
  "word": "spin",
  "phonetic": "/spɪn/", // The pronunciation of the word using the International Phonetic Alphabet(IPA)
  "phonetics": [
    {
      "text": "/spɪn/",
      "audio": "https://api.dictionaryapi.dev/media/pronunciations/en/spin-au.mp3"
    }
  ],
  "meanings": [
    {
      "partOfSpeech": "noun",
      "definitions": [
        {
          "definition": "Rapid circular motion.",
          "synonyms": [], // No synonyms provided for this definition.
          "antonyms": [], // No synonyms provdied for this definition.
          "example": "He put some spin on the cue ball."
        }
      ]
```
***Note:** Response abbreviated -- the full response also includes a "verb" sense of spin, plus additional phonetics, licensing info, and source URLs. Every response includes synonyms/antonyms arrays even when empty.*
 
## Error Handling
| **Code** | **Error** | **Descriptions** |
| -------- | --------- | ---------------- |
| 522| Connection Timed Out | The request could not reach the API server.

***Note:** During testing, every invalid request -- missing parameters, misspelled words -- returned the same ``` 522 Connection Timed Out ```  rather than a distinct word-specific error response. The API does not differentiate error causes in its response*
## Try it
If you keep receiving the ``522 Connection Timed Out``  error, double-check your word and language code for typos first. If the error persists, it might be from the API's end -- wait a few minutes and try again.
