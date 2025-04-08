## Setup

### 1. Prerequisites
- [Scriptable App](https://apps.apple.com/us/app/scriptable/id1405459188)
- iOS 16+ with Lock Screen widget support

### 2. Add These Scripts to Scriptable

| Script Name              | Purpose                                 |
|--------------------------|------------------------------------------|
| `Lockscreen Weather`     | Displays weather with emoji + vibe       |
| `Update Weather Location`| Gets your current GPS silently           |

> You can paste each script into a new file in Scriptable.

### 3. Add Shortcuts (Optional but Recommended)

Use the **Shortcuts** app to add a quick GPS refresh button:

1. Open the **Shortcuts** app
2. Tap **+**, name it something like `Update Weather`
3. Add action: **Run Script**
4. Choose script: `Update Weather Location`
5. Save the shortcut
6. Add it to your Lock Screen as a shortcut button for manual refresh

### 4. Automation (Optional)

You can also auto-refresh your location every time **Scriptable** opens:

1. Go to the **Shortcuts** app → Automations
2. Create a new **Personal Automation**
3. Trigger: **When “Scriptable” is opened**
4. Actions:
   - Run Script → `Update Weather Location`
   - (Optional) Run Script → `Lockscreen Weather`
5. Turn OFF "Ask Before Running" and "Notify When Run"

### 5. Add the Widget

1. Long press your Lock Screen → **Customize**
2. Tap **Add Widget** → Select **Scriptable**
3. Choose the `Lockscreen Weather` script