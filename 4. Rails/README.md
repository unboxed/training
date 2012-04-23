# Rails

After teaching Rack applications, we move onto Rails.

## Preliminary Content

* App tour
* Stack
* Web-MVC
* ActiveSupport

## Testing

* Why do we test?
* Approaches for testing
* What to test?
* Test Unit + mocking
* RSpec
* Factories
* Cucumber + class-level macros
  * Do it with acceptance testing and integration
  * Capybara
  * Webrat

## Things to remember

* Our end goal is test-driven development

## Practical Delivery

The RoR course content will be delivered through the development of a simple Rails app. The simple app will:

Use ActiveRecord
Have problems that can be resolved through the use of a gem (e.g. pagination)
* Use CRUD
* Have forms
* Be integrated with a social media API (Gravatar)
* Be a simple version of something that already exists (e.g. Reddit, Stack Overflow)

The simple app will not:

* Require authentication
* Have a CMS (admin section)

Although these could be extensions

## Rails app overview

Stories are:

As a user, I want to submit an entry (A/C: contains a title, body, email address of the submitter, submit button, saved in DB) [Medium]

As a user, I want to see a list of submitted entries (A/C: index sorted by submit date - newest first, title, email, date submitted) [Medium]

As a user, I want pagination of submitted entries (A/C: 10 per page, first and last page, jump to new page - ajax enhancement potential) [Small]

As a user, I would like to see a Gravatar instead of an email address (A/C: see gravatar on entry page and index, it is correct and is sized correctly) [Medium]

Interns will have written Acceptance tests. When you switch to using the gem for Gravatar, the tests should pass without re-implementation (hopefully)

As a user, I want to comment on an entry (A/C: Can comment on any entry, see Gravatar next to comment, see time of comment) [Medium]

Extension stories

As a user, I want to vote on an entry (A/C: results in sorting, up and down voting, vote count presented - using ajax => progressive enhancement changes in back-end) [Large]

As a user, I want to vote on a comment (A/C: results in sorting, up and down voting, vote count presented - using ajax => progressive enhancement changes in back-end) [Large]

As a user, I want to be able to authenticate myself - has_secure_password, rails basic auth, devise (Tutor should demonstrate code - probably won't be implemented)
