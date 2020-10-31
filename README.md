# Skeleton for new Rails 5 application for REST API

[![Build Status](https://semaphoreci.com/api/v1/ezedepetris/place-to-park-api/branches/master/badge.svg)](https://semaphoreci.com/ezedepetris/place-to-park-api)

This simple application includes Ruby/Rails technology which we use at Flatstack for new REST API projects. Application currently based on Rails 5 stable branch and Ruby 2.5.1

## What's included

### Application gems:

* [puma](https://github.com/puma/puma) as Rails web server

### Development gems

* [dotenv](https://github.com/bkeepers/dotenv) - load environment variables from `.env`

### Testing gems

* [factory bot](https://github.com/thoughtbot/factory_bot) - create test data
* [faker](https://github.com/stympy/faker) - generate fake data
* [rspec api documentation](https://github.com/zipmark/rspec_api_documentation) - generate pretty API docs
* [rspec](https://github.com/rspec/rspec) - awesome, readable isolation testing
* [shoulda matchers](http://github.com/thoughtbot/shoulda-matchers) - frequently needed Rails and RSpec matchers

### Scripts

* `bin/setup` - build Docker image and prepare DB
* `bin/server` - to run server locally
* `bin/ci` - runs RSpec tests and quality tools

## Quick start

Clone application as new project with original repository named "place-to-park-api"

```bash
git clone git://github.com/ezedepetris/place-to-park-api.git --origin place-to-park-api [MY-NEW-PROJECT]
```

Create your new repo on GitHub and push master into it.
Make sure master branch is tracking origin repo.

```bash
git remote add origin git@github.com:[MY-GITHUB-ACCOUNT]/[MY-NEW-PROJECT].git
git push -u origin master
```

Run setup script

```bash
bin/setup
```

Make sure all test are green

```bash
bin/ci
```