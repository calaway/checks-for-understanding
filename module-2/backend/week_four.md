## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
  * A packet of information from a website that your browser stores for a predetermined amount of time.
* What’s the difference between a session and a cookie?
  * Sessions are generally encrypted and expire when the browser closes.
* What’s a flash and when do you want to use flashes?
  * Flash stores info until it is called once and then is cleared.
* Why do people say “HTTP is stateless”?
  * HTTP requests are always independent of any other HTTP request. They are not able to store any information from one to the next.
* What’s authentication? Explain.
  * Verifying that your users are who they say they are.
* What’s the difference between authentication and authorization?
  * Authorization requires that authentication has already happened. It means that you allow users to see pages they should have access to and block the ones they shouldn't.
* What’s a before filter?
  * A method that runs before each action in a controller, unless you limit it only to specific actions.
* How do we keep track of a user once they’ve logged in?
  * Store a session
* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
  * Namespacing a resource only involves a single resource, while nesting involves two. Namespacing could be used to show a different users index page to an admin vs a regular user. Nesting could be used when one resource is completely dependent on another.
* At a high level, what tools can you use to implement authorization? How would you use them?
  * Assign users a role and only allow them access to pages for which that role is sufficient.
* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
  * I don't know.
* What are some strategies you can use to keep your views DRY?
  * Creating partials or helper methods in your controller
