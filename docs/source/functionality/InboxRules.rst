Inbox Rules
=======
Inbox rules process messages in the inbox based on conditions and take actions such as moving a message to a specified folder or deleting a message.

Show mailbox rules
^^^^^^^^^^^
**Show-MailboxRules** shows the mailbox rules in your organization.

Usage
""""""""""""""""""""""""""
Show all mailbox rules in your organization:
::

   Show-MailboxRules

Show the mailbox rules for the users test[@]invictus-ir.com and HR[@]invictus-ir.com:
::

   Show-MailboxRules -UserIds "HR@invictus-ir.com,test@Invictus-ir.com"

Parameters
""""""""""""""""""""""""""
-UserIds (optional)
    - UserIds is the UserIds parameter filtering the log entries by the account of the user who performed the actions.

Get mailbox rules
^^^^^^^^^^^
**Get-MailboxRules** collects all the mailbox rules in your organization.

Usage
""""""""""""""""""""""""""
Get all mailbox rules in your organization:
::

   Get-MailboxRules

Get the mailbox rules for the user test[@]invictus-ir.com:
::

    Get-MailboxRules -UserIds Test@Invictus-ir.com

Get the mailbox rules for the users test[@]invictus-ir.com and HR[@]invictus-ir.com:
::

   Get-MailboxRules -UserIds "HR@invictus-ir.com,test@Invictus-ir.com"

Parameters
""""""""""""""""""""""""""
-UserIds (optional)
    - UserIds is the UserIds parameter filtering the log entries by the account of the user who performed the actions.

Output
""""""""""""""""""""""""""
The output will be saved to the 'Rules' directory within the 'Output' directory, with the file name 'MailboxRules.csv'.
