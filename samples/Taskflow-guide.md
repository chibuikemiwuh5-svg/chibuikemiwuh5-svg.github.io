# How to Set Up Custom Notifications in TaskFlow

TaskFlow's default notifications alert you to every comment, status change, and mention across all your projects — which can quickly become noise. Custom notification rules let you choose exactly what you're notified about, and how.

This guide walks you through creating a custom rule in under five minutes.

## Before you start

- You'll need a TaskFlow account with at least **Member** access to the project you want to customize.
- Custom rules apply per-project. If you manage multiple projects, you'll repeat this process for each one.

## Step 1: Open your notification settings

1. Click your profile icon in the top-right corner.
2. Select **Settings > Notifications**.
3. Choose the project you want to customize from the dropdown at the top of the page.

## Step 2: Create a new rule

1. Click **+ New Rule**.
2. Give the rule a short, descriptive name (for example, "Only my tasks" or "Deadline alerts").
3. Under **Trigger**, choose the event that should activate this rule:
   - Task assigned to me
   - Due date within 24 hours
   - Status changed to "Blocked"
   - Comment added to a task I'm watching

## Step 3: Choose how you're notified

For each rule, select one or more delivery methods:

| Method | Best for |
|---|---|
| In-app banner | Low-priority updates you'll check later |
| Email | Anything you need a paper trail for |
| Slack/Teams alert | Time-sensitive items, like blockers |

**Tip:** Reserve email and chat alerts for high-priority triggers. Overusing them defeats the purpose of custom rules.

## Step 4: Set quiet hours (optional)

To avoid after-hours pings:

1. Toggle **Respect quiet hours** on.
2. Set your active hours (for example, 9 AM–6 PM).
3. Notifications triggered outside this window are held and delivered in a single digest at the start of your next active period.

## Step 5: Save and test

1. Click **Save Rule**.
2. To confirm it works, trigger the event yourself — for example, assign a test task to yourself if that's your chosen trigger.
3. You should see the notification arrive via your selected method within a minute.

## Troubleshooting

**I'm not receiving notifications.**
Check that the rule is toggled **On** (rules are saved as off by default) and confirm your email or Slack integration is still connected under **Settings > Integrations**.

**I'm getting duplicate notifications.**
This usually means two rules overlap — for example, one rule for "Task assigned to me" and another for "Any activity on my tasks." Review your rules list and remove the redundant one.

**Quiet hours aren't holding notifications.**
Quiet hours only apply to rules created after the feature was enabled on your account. Re-save any older rules to apply the setting retroactively.

---

*Have a rule that's not covered here? Reach out to support@taskflow.example, and we'll help you fine-tune it.*
