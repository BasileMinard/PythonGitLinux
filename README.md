Git interactive rebase
Many times, when working with Git, you may want to revise your local commit history. One of the great things about Git is that it allows you to make decisions at the last possible moment. You can decide what files go into which commits right before you commit with the staging area, you can decide that you didn’t mean to be working on something yet with git stash, and you can rewrite commits that already happened so they look like they happened in a different way.
To modify a commit that is farther back in your history, you must move to more complex tools. One of the most useful tools for this is an interactive rebasing script. This process allows you to stop after each commit you want to modify and change it however you wish — the commit message, the snapshot, or both.

Changing Multiple Commit Message
You can run an interactive rebase by passing the -i option to git rebase. You must tell Git how far back you want to rewrite commits by telling it which commit to rebase onto. For example, if you want to edit the last three commits, or the commit HEAD~3, you would run git rebase -i HEAD~3.

-- sherynne
