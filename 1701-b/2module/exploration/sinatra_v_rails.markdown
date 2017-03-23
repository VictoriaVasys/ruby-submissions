## Sinatra versus Rails Exploration

### Setup:

First, clone down the Rails project:

```terminal
git clone https://github.com/turingschool/job-tracker.git rails_project
```

And then clone down the Sinatra project:

```terminal
git clone https://github.com/turingschool/bike-share.git sinatra_project
```
Now cd into each project, run `bundle` on each project, and you're ready to go. We will only be looking at the code base and not interacting with the app. If you wanted to run the server and interact with the app, you would need to create your database, migrate your migrations, etc.

### Exercise:

1. Take a look at this stripped down Sinatra app and this stripped down Rails app. How are they different and how are they similar? Identify 5 differences, and for each one describe 1-2 implications. What effect does that difference have for each framework? If you don't know exactly, draw on your knowledge and experience and make some educated guesses/inferences. Also, practice your research skills to look into the differences.


The Root of the Rails project has additional directories of `bin`, `lib`, `log`, `public`, and `vendor`
The Rails `config` directory has additional directories `environments`, `initializers`, and `locales` and additional files of `application.rb`, `boot.rb`, and `routes.rb`
The `app` directory in Rails project has assets, helpers, and mailers in addition to MVC.
The Rails project has a `rails_helper.rb` file, which defines...
The `public` directory contains html files that dictate content when there are client or server errors (4xx or 5xx HTTP response codes).


1. Consulting blogs and commentary you find online, identify 3 similarities between Rails and Sinatra.

They are both frameworks to build web apps with Ruby, both utilize the MVC model, and can work with databases/SQL.

1. Consulting blogs and commentary you find online, identify 3 things that distinguish Rails, advantages.

Rails has an API Controller that can handle APIs and abstract them from the controller, is more robust and can handle a lot (especially architecture & tooling), and has a templating language that allows you to generate HTML files, routing, plugins and more.

1. In your Rails project, what does the `routes.rb` file inside of the `/config` directory do? What does this correlate to in our Sinatra app?

The routes file seems to be able to handle client requests the way our controller did in Sinatra.

1. We teach Sinatra by adding some structures that Sinatra doesn’t need, but help you make the transition between Sinatra and Rails. What does a stripped down implementation of Sinatra look like, and what are the pieces we’ve added for educational purposes?

Stripped-down is simply MVC model; you do not need a public folder (do not need to publish), nor do you have to use databases
