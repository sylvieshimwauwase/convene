this project aims to create a convene app

Convene assists meetup organisers in prioritising questions to be answered by allowing users to vote on them. The most popular questions are displayed at the top.


Required Features
1. Admin can create meetups.
2. Users can create an account and log in.
3. Users can post questions to a specific meetup.
4. Users can upvote or downvote a question.
5. Questions are sorted based on the number of upvotes a question has, which helps the meetup organizer(s) to prioritize questions most users are interested in.
6. Users can post comments to a specific question.
Optional Features
1. Admin can add images to a meetup record.
2. Admin can add tags to a meetup record.
3. The user can reset password.


Preparation Guidelines
These are the steps you ought to take to get ready to start building the project
Steps
1. Create a Pivotal Tracker/ Trello Board
2. Create a Github Repository, add a README, and clone it to your computer


Challenge One Summary
You are required to create UI templates with HTML, CSS, and Javascript (React).

NB:
● You are not implementing the core functionality yet, you are only building the User Interface (UI) elements, pages, and views!
● You are to create a pull request for each feature in the challenge and then merge into your develop branch.
● Do not use any CSS frameworks, e.g. Bootstrap, Materialize, sass/scss.
● Do not download or use an already-built website template. 
Guidelines
1. On Pivotal Tracker, create user stories to setup the User Interface (UI) elements:
a. User sign-up page.
b. User sign-in page.
c. A page/pages where a user can do the following:
i. Post a question to a specific meetup.
ii. Upvote and Downvote a question.
iii. Add a comment to a question.
d. A page/pages for a user’s profile which, at minimum displays:
i. The number of questions the user has posted.
ii. The number of questions the user has commented on.
iii. Top questions feed for upcoming meetup(s) that the user is scheduled to
attend.
e. A page/pages where an Admin can do the following:
i. Create a meetup.
ii. Delete a meetup.
2. On Pivotal Tracker, create stories to capture any other tasks not captured above. A
task can be feature, bug or chore for this challenge.
3. On a feature branch, create a directory called UI in your local Git repo and build out all
the necessary pages specified above and UI elements that will allow the application
function into the UI directory
4. Host your UI templates on GitHub Pages.
Tip: It is recommended that you create a gh-pages branch off the branch containing your
UI template. When following the GitHub Pages guide, select "Project site" >> "Start from
scratch". Remember to choose the gh-pages branch as the source when configuring
Repository Settings.
Challenge 2: Create API endpoints
Challenge Summary
You are expected to create a set of API endpoints defined in the API Endpoints Specification
section and use data structures to store data in memory (don’t use a database).
Timelines
● Duration: 1 Week
● Due Date: 4th January, 2019
NB:
● You are to create a pull request for each feature in the challenge and then merge into
your develop branch
Tools
● Server side Framework: Node/Express
● Linting Library: ESLint
● Style Guide: Airbnb
● Testing Framework: Mocha or Jasmine
Guidelines
1. Setup linting library and ensure that your work follows the specified style guide
requirements.
2. Setup the test framework.
3. Write unit-tests for all API endpoints.
4. Version your API using URL versioning starting, with the letter “v”. A simple ordinal
number would be appropriate and avoid dot notation such as 2.5. An example of this
will be: https://somewebapp.com/api/v1/users.
5. Using separate branches for each feature, create version 1 (v1) of your RESTful API to
power front-end pages.
6. On Pivotal Tracker, create user stories to setting up and testing API endpoints that do
the following using data structures:
○ Create a meetup record.
○ Create a question record.
© Andela Confidential
○ Get a specific meetup record.
○ Get all meetup records.
○ Upvote or downvote a question.
○ Rsvp for a meetup.
7. On Pivotal Tracker create stories to capture any other tasks not captured above. The
tasks can be feature, bug or chore for this challenge.
8. Setup the server side of the application using the specified framework
9. Ensure to test all endpoints and see that they work using Postman.
10. Integrate TravisCI for Continuous Integration in your repository (with ReadMe badge).
11. Integrate test coverage reporting (e.g. Coveralls) with a badge in the ReadMe.
12. Obtain CI badges (e.g. from Code Climate and Coveralls) and add to ReadMe.
13. Ensure the app gets hosted on Heroku.
14. At the minimum, you should have the API endpoints listed under the API endpoints
specification on page 13 working. Also refer to the entity specification on page 12 for
the minimum fields that must be present in your data models.
API Response Specification
The API endpoints should respond with a JSON object specifying the HTTP status code, and
either a data property (on success) or an error property (on failure). When present, the data
property is always an array, even if there’s none, one, or several items within it.
On Success
{
“status” : 200,
“data” : [{...}]
}
On Error
{
“status” : 404,
“error” : “relevant-error-message”
}
The status codes above are provided as samples, and by no way specify that all success
reponses should have 200 or all error responses should have 400.

