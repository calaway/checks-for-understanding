## Week Three Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What are the 3 main features in an ERD?
  * Concrete objects, organizations, abstract objects
2. Create an ERD for the following database: Restaurants, Customers, Items, Ingredients, Beverages, Orders, Vendors.
3. What is the entry at the command line to create a new rails app?
  * rails new app_name
4. What do Models generally inherit from in rails?
  * ActiveRecord::Base (through ApplicationRecord in version 5)
5. What do Controllers generally inherit from in a rails project?
  * ActionController::Base (through ApplicationController)
6. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
  * resources :horses, only: [:show]
7. What rake task is useful when looking at routes, and what information does it give you?
  * rake routes
8. What is an example of a route helper? When would you use them?
  * Example: `new_artist` routes to `/artists/new`. You can use these with link_to.
9. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
  * `_path` will only return the relative path, while `_url` will return the full url
10. What are strong params and why are the necessary?
  * Strong params are used to protect your app from users submitting bogus params with nefarious intent.
11. What role does `form_for` play in helping us create our forms?
  * It gives us a simpler way to build out a form, rather than using just html.
12. How does `form_for` know where to submit the user's input?
  * It takes an argument and you pass where it should be submitted to
13. Create a form using a `form_for` helper to create a new `Horse`. 
```ruby
<%= form_for(@horse) do |f| %>

  <%= f.label :name %>
  <%= f.text_field :name %>

  <%= f.label :breed %>
  <%= f.text_field :breed %>

  <%= f.submit %>
<% end %>
```
14. Why do we want to validate our models?
  * To ensure that the record is only created if it is valid
