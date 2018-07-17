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

  * `todo.sh due` - list tasks sorted by due date 
  * `todo.sh due list` - same as above 
  * `todo.sh due set <#item> <due_date>` - set the due date on task `<#item>` to `<due_date>`
  * `todo.sh due unset <#item>` - remove due date from task `<#item>`
