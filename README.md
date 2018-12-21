# Travis CI monorepo Demo [![Build Status](https://travis-ci.org/arnaskro/monorepo-travis.svg?branch=master)](https://travis-ci.org/arnaskro/monorepo-travis)

This repository is an experiment about building monorepo projects using [Travis CI](http://travis-ci.org/).

Be sure to checkout my [Circle CI monorepo demo](https://github.com/arnaskro/monorepo-circleci) if you are interested in other CI options.

## How it works?
It makes use of Travis matrix feature where in `.travis.yml` we define folders to different project locations in the repo.
What happens next is when Travis runs the build it creates a job for each defined project.
Then in each job it checks if the project has changes using `git diff` and runs tests if it does.
