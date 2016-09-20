# Continuous integration and deployment with GitHub, Travis and Heroku

## Deploy to Heroku

1. Create app on Heroku and set up Git remote: `heroku create`
1. `git push heroku master`
1. add any necessary environment variables
1. Set up db on Heroku `heroku addons:create heroku-postgresql:hobby-dev`
1. Update knexfile w/ production config
1. Push to heroku, after commit
1. migrations `heroku run knex migrate:latest --env=production`
1. seeds
1. `heroku restart`

## Push to GitHub

1. set up remote on GitHub
1. push
