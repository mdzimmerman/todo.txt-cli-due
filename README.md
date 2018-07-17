# todo.txt CLI due

Adds a "due" command to todo.sh for mananging due dates on tasks.

## Installation 

Prequisites: Python, dateutil

Copy or symlink the `due` executable into `./.todo.actions.d`.

## Use

In the commands below, `<due_date>` can include any date format parsable by
`dateutil.parser.parse()`; including:

  * "today"
  * "tomorrow"
  * "friday"
  * "fri"
  * "jul 20"

Due dates are stored by appending the string "due:YYYY-MM-DD" to tasks.

## Commands

  * `todo.sh due` - summarize overdue tasks, tasks due in the next week, and tasks without due dates
  * `todo.sh due add` - create a new task with default due date of today
  * `todo.sh due list` - list overdue tasks and tasks due today
  * `todo.sh due set <#item> <due_date>` - set the due date on task `<#item>` to `<due_date>`
  * `todo.sh due summarize` - same as `todo.sh due`
  * `todo.sh due unset <#item>` - remove due date from task `<#item>`
  * `todo.sh due usage` - print usage
