#how-to-rated-r

Restoring a LÖVE repository's previous name is super simple.

## Licensing concerns

Make sure you only do this if the repo's license allows it.

That's really the only concern though! Let's get on with it.

## Basic method

Navigate to the repository, fork it under "love-rated-r", and edit the name of the repo.

Someone else will attempt to keep the repoes up to date (although you're welcome to help!)

## Advanced method

Sometimes the repository owners modify files in the repository to reflect the name change. This requires a little more effort, but it's still really simple!

(Also, make sure you've completed the Basic part above first.)

First, `git clone` the fork locally.

Then, disguise your email address and name by running the snippet below inside the repo:
```
git config user.name "Significant Lover"
git config user.email "loveratedr@tfwno.gf"

```

Then, use Git tools to undo changes. `git checkout <sha1 hash of unedited commit> <filename>` until the edits are all gone.

Finally, `git commit -m "Revert changes"` and `git push`! You're all done!

Please note that you shouldn't edit files by hand, but rather cherry-pick them with `git checkout`. This helps avoid politicized editing, when the only goal is to restore the names of the repositories.

If you have any questions, comments, or concerns; please get in touch at [loveratedr@tfwno.gf](mailto:loveratedr@tfwno.gf).

