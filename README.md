# git-merge-example

This repo shows that when merging from one branch to another conflicts that
were previously resolved in one merge do not need to be resolved again in
subsequent merges.

The sequence of steps are.

1. master add file filea, with conent `a`
1. checkout branch called branch and change filea content to `b`
1. master add content on new line to filea
1. branch merge master and resolve the conflict `a` vs `b` select our change `b`
1. master add more content on a newline to filea
1. branch merge master again and witness no conflict
