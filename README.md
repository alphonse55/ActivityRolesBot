# Activity-Roles-Bot
- load token
- instantiate the bot

in on_ready():
- get the guild, channels, and members_who_aren't_bots into variables
- create the message_count dict for members who are not bots
- put the activity roles into a variable

- load numbers into message_count dict from a file (encapsulate into a function)
- load last save time (encapsulate into a function)

- iterate through the channels, iterating through the history from the last save time, and add to the members' counts

- remove all activity roles from the members who are not bots
- add activity roles where appropriate

in on_message():
-add one to the count of the member
-if a change should happen to the member's role, remove the previous activity roles and then add the new one
