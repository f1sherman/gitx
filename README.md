# thegarage-gitx

[![Build Status](https://travis-ci.org/thegarage/thegarage-gitx.png?branch=fix-rspec-mocks)](https://travis-ci.org/thegarage/thegarage-gitx)

Useful Git eXtensions for Development workflow at The Garage.

Inspired by the [socialcast-git-extensions gem](https://github.com/socialcast/socialcast-git-extensions)

# Git Extensions for Workflow

### Options
* `-v` = verbose for debugging commands

## git start <new_branch_name (optional)>

update local repository with latest upstream changes and create a new feature branch

## git update

update the local feature branch with latest remote changes plus upstream released changes.

## git integrate <aggregate_branch_name (optional, default: staging)>

integrate the current feature branch into an aggregate branch (ex: prototype, staging)

## git reviewrequest

create a pull request on github for peer review of the current branch.

## git release

release the current feature branch to master.  This operation will perform the following:
* pull in latest code from remote branch
* merge in latest code from master branch
* prompt user to confirm they actually want to perform the release
* merge current branch into master
* cleanup merged branches from remote server

# Extra Utility Git Extensions

## git cleanup

delete released branches after they have been merged into master.

## git nuke <aggregate_branch_name>

reset an aggregate branch (ex: prototype, staging) back to a known good state.


## Note on Patches/Pull Requests

* Fork the project.
* Make your feature addition or bug fix.
* Add tests for it. This is important so I don't break it in a
  future version unintentionally.
* Commit, do not mess with rakefile, version, or history.
  (if you want to have your own version, that is fine but bump version in a commit by itself I can ignore when I pull)
* Send me a pull request. Bonus points for topic branches.

## Copyright

Copyright (c) 2013 The Garage, Inc. See LICENSE for details.