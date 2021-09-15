`git stash`

to see the stashed stuff
`git stash list`

to see the diffs stash wise
`git stash show -p stash@{1}`

to apply changes of a particular stash
`git stash apply stash@{1}`

see all diff of stashes
` git diff stash^!`

create new branch with stashed changes
`git stash branch <branchname> [<stash>]`
