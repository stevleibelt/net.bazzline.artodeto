# Content of the blog

Free as in freedom collection of links and link description.

The current change log can be found [here](CHANGELOG.md).

# Todo

* Add a bin that cleans the history
  * Only the history of the last year (with all its commits) should be visible
  * If there is a full year available
    * Put all this commits into
      * One tag
      * One commit

```bash
# fetch git log between two dates
git log --since "DEC 1 2014" --until "DEC 5 2014"
# rebase last four commits on top of HEAD
git rebase HEAD~4

# As example
# Fetch latest commit id for date in the past
git log --until "DEC 31 2017"  --pretty=format:"%h" | head -n 1
# Fetch number of commits available in the past
git log --until "DEC 31 2017" | grep -c commit
```
