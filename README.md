# doodle-qa-backend-challenge
The API tests were written in Postman and can be run using Newman. I was only able to automate the happy path for the endpoints and given more time, I would have been able to figure out and automate all the test cases I came up with.

To run the test, 

1. Download and install Node.js.

2. Run the command "npm install -g newman" in your CLI.

3. Run the command "newman run OpenAPI definition.postman_collection"



# The test cases I came up with

User:

- Create a user with a unique name
- Create a user with an existing name
- Get all created users
- Get a specific user
- Delete all users
- Delete specific user
- Get deleted user
- Test pagination

Slot:
- Create a slot with valid start and end time
- Create a slot with end time earlier than start time
- Create a slot without start and end time
- Create a slot with the same start and end time
- Create a slot without start time
- Create a slot without end time
- Get all created slots
- Get specific slot
- Delete specific slot
- Get deleted slot

Meeting:
- Create a meeting with one slot
- Create a meeting with multiple slots
- Create a meeting without a slot
- Create a meeting without a title
- Create a meeting without a participant
- Create a meeting with one participant
- Create a meeting with multiple participants
- Create a meeting with already used slots
- Get a created meeting
- Get all created meetings
- Delete a meeting
- Get deleted meeting

Calendar:
- Get calendar for a month in the past
- Get calendar for a month in future
