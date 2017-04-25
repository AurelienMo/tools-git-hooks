# Hooks GIT pre-commit
## Requirements
**phpcs**  
Global install required with standard Symfony2

**phpmd**  
Global install with all ruleset at this [url](https://github.com/AurelienMo/tools-phpmd)

**phpunit**  
Install from vendor

## Execute
On each commit, hook check:
- if **phpcs** with standard Symfony2 is ok
- if **phpmd** with phpmd_symfony ruleset is ok
- if unit tests with **phpunit** is already ok

If an error has been occured during execute, commit is denied and the error is displayed in the console.