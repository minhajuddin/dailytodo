# Daily TODO

A simple, elegant daily task tracker with support for day-specific tasks and visual organization.

## Features

- ✅ Daily task tracking with completion status
- 📅 Day-specific tasks (show tasks only on certain days)
- 📊 History view to track your progress over the last 7 days
- 💾 Automatic local storage (no sync required)
- 📱 Responsive design works on desktop and mobile

## Getting Started

1. Open `index.html` in your web browser
2. Click the "Edit List" tab
3. Enter your tasks, one per line
4. Click "Save" to update your task list
5. Return to the "Today" tab to see your tasks for the day

## Task Format

### Basic Tasks

Simply enter one task per line:

```
Buy groceries
Finish report
Call mom
Exercise
```

### Named Sections

Create organized sections with visual headers using `--- Section Name ---`:

```
--- Morning Routine ---
Make coffee
Shower
Review calendar

--- Work Tasks ---
Check emails
Team standup
Project work

--- Evening ---
Cook dinner
Read
Wind down
```

Named sections will display as colored headers in your task list and help organize your tasks into logical groups.

### Spacers

Create simple visual divisions between groups using `---` on its own line:

```
Buy groceries
Walk the dog
---
Finish report
Review emails
---
Call mom
Exercise
```

You can combine spacers with named sections for maximum flexibility.

### Day-Specific Tasks

Add tags to tasks to show them only on certain days. Use day names, `#weekday`, or `#weekend`:

```
Morning Jog #weekday
Brunch with friends #weekend
Team Meeting #monday #wednesday #friday
Laundry #saturday
Rest Day #sunday
Grocery Shopping #weekday
```

#### Available Tags

- **Day names**: `#monday`, `#tuesday`, `#wednesday`, `#thursday`, `#friday`, `#saturday`, `#sunday`
- **Day groups**: `#weekday` (Mon-Fri), `#weekend` (Sat-Sun)
- **No tag**: Task appears every day

#### Tag Examples

```
Morning yoga #weekday        # Shows Mon-Fri only
Team standup #monday #wednesday #friday
Meal prep #sunday            # Shows Sunday only
Daily reading               # Shows every day (no tags)
Brunch #saturday #sunday    # Shows on weekends
```

### Combined Example

Here's a complete task list combining all features:

```
--- Morning Routine ---
Make coffee
Review calendar
Meditation

--- Weekday Work ---
Check emails #weekday
Team standup #monday #wednesday #friday
Project work #weekday

--- Weekend Activities ---
Sleep in #weekend
Brunch #weekend
Laundry #saturday
Meal prep #sunday

--- Evening ---
Exercise
Read
Wind down
```

This example uses:
- **Named sections** (`--- Section Name ---`) to organize tasks visually
- **Day-specific tags** (`#weekday`, `#saturday`, etc.) to show tasks only on certain days
- **Basic tasks** that appear every day

## Tabs

### Today
Shows tasks for the current day, filtered by day-specific tags. Check off completed tasks.

### Edit List
Edit your master task list. Changes are saved automatically when you click "Save".

### History
View your task completion history for the last 7 days, including:
- Completion percentage for each day
- Which tasks you completed vs. didn't complete
- Only shows tasks that applied to each specific day

## Tips

- Tasks without tags appear every day
- Spacers (`---`) help organize your list visually
- You can use multiple tags on a single task: `Team meeting #monday #wednesday #friday`
- History respects day-specific tags, so weekend-only tasks don't count against your weekday stats
- Your data is stored locally in your browser - no internet required after the first load

## Storage

All data is stored in your browser's local storage:
- `dailytodo_masterlist`: Your task list
- `dailytodo_completions`: Task completion history by date

Clear your browser's local storage if you want to reset the app.
