# Memory bank management

The memory bank is a feature intended to document progress of a coding session for using it at the beginning of the next one for easier, quicker onramp and token saving by avoiding having to run a full analisys of the project from the get go.

## File management

- You will be managing a single file named `memory_bank.md` usually located at the root of the current project, unless the user specifies otherwise.
- `memory_bank.md` contains a specific file structure detailed below.
- `memory_bank.md` will be written into and emptied based on this command arguments you are provided.
- if `memory_bank.md` does not exist, you will create it.

## Session management

Based on `$ARGUMENTS`, the actions to take are:

- $ARGUMENTS == "read": read and internalize the contents of the `memory_bank.md`. This will give you context on the last actions you performed and what are the inmediate next steps to take. Once you have read and understood the follow up actions, acknowledge it and return the user a TO DO list based on it.
- $ARGUMENTS == "write": save the current session progress into the `memory_bank.md`. This will include completed tasks, immediate next actions, and any critical decisions made during the session. Use the structured format provided below. Once the contents are saved, acknowledge it and return the user a confirmation message.
- $ARGUMENTS == "clear": clear the contents of the `memory_bank.md`.
- if $ARGUMENTS has any other value, return an error message indicating that the argument is invalid and showing the valid options.

## Memory Bank File Structure

```markdown
# Memory Bank

## Current Status

Last Updated: [Current Date and Time]

## Completed This Session

- [Specific achievement 1]
- [Specific achievement 2]

## Next Immediate Actions

- [Priority 1 task]
- [Priority 2 task]

## Critical Context

[Any important decisions or constraints, known issues, or future considerations]
```
