# Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Open]

### To Add

* [squash](https://opensource.com/article/22/4/manage-git-commits-rebase-i-command) commits
    * one per week for weeks older than 3 months
    * also check [git amend](https://opensource.com/article/22/4/git-tips)
    * `git rebase -i <branch>`
    * Or
    * `git rebase -i --root`
      * See [this](https://opensource.com/article/22/11/advanced-git-commands) or [that](https://opensource.com/article/22/11/git-tips-technical-writers) `git rebase -i` information
    * Or
      * Copy content without .git into new directory
        * Pull all commits from 01.01.yyyy until 31.12.yyyy and commit dem as one
        * Pull all commits from current year and commit them as one
    * If any of this ideas is working, apply it to all the other repositories like general_howts etc.
* bin/calendar_week
    * check if latest draft file is current or last week
    * if latest draft is current week
        * create new draft with +1 of current calendar week
    * else
        * create new draft file with current calendar week

### To Change

* fix the issue that the last draft file from previous year will never be renamed to non draft

## [Unreleased]

### Added

* Added execution of >>git gc --aggressive<< when [calendar_week](bin/calendar_week) is executed

### Changed

* Moved core logic in [calendar_week](bin/calendar_week) into function `_main`

