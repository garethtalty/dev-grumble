---
title: Crafting the Perfect Git Commit
date: 2021-01-28 15:40:11
tags:
  - git
  - tips
  - productivity
  - code review
---

![](images/git-commit.jpg)
<figcaption>
  <span>Photo by <a href="https://unsplash.com/@yancymin?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Yancy Min</a> on <a href="https://unsplash.com/s/photos/git?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a></span>
</figcaption>

You probably already use git for source control and are probably very familiar with `git add`.

Perhaps you haven’t yet discovered a very simple way to keep your commits small and meaningful…

Pass the `-p` or `--patch` option to git add and git will split your files into ‘hunks’ and present a diff for each hunk, one at a time with various options:
```
y - stage this hunk
n - do not stage this hunk
a - stage this and all the remaining hunks in the file
d - do not stage this hunk nor any of the remaining hunks in the file
g - select a hunk to go to
/ - search for a hunk matching the given regex
j - leave this hunk undecided, see next undecided hunk
J - leave this hunk undecided, see next hunk
k - leave this hunk undecided, see previous undecided hunk
K - leave this hunk undecided, see previous hunk
s - split the current hunk into smaller hunks
e - manually edit the current hunk

? - print help
```

Using `git add -p` in this way allows you to create small, sensible commits that are very focused. Additionally, it gives you an opportunity to self-review your changes as you add, win-win!

## Further reading
https://git-scm.com/book/en/v2/Git-Tools-Interactive-Staging#Staging-Patches


## Acknowledgement
_Originally published by Gareth Talty on behalf of [Gousto](https://www.gousto.co.uk) at [techbrunch.gousto.co.uk](https://techbrunch.gousto.co.uk/2017/01/18/git-add-p/) on January 18, 2017._
