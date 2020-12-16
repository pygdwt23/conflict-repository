# Conflict di Repository

### Apa saja yang menyebabkan terjadinya conflict?
Karena kode yang kita tulis berbeda dengan yang lain.

Misalnya, Si A menulis kode untuk fitur X dengan algoritma yang ia ketahui. Sedangkan si B menulis dengan algoritma yang berbeda.

Lalu mereka melakukan commit, dan kode sumber jadi berantakan. Anggota tim yang lain menjadi pusing.

![https://www.petanikode.com/git-branch/](https://2.bp.blogspot.com/-DEigCiYJJfY/WLMaWoeoONI/AAAAAAAAELQ/qvDUmoiDWQMElIHdl8y4qkT0ZsjDk6TzQCPcB/s1600/konflik-branch-repositori-git.png)

### Bagaimana menghindari conflict?
-  Menggunakan Percabangan untuk Menghindari Konflik
###
Perintah untuk membuat cabang adalah git branch, kemudian diikuti dengan nama cabangnya.
```
git branch fitur_register
```
Maka Git akan membuat cabang bernama fitur_register.
![https://www.petanikode.com/git-branch/](https://4.bp.blogspot.com/-A8Ps8Hfz-Wg/WLMdwfZK7WI/AAAAAAAAELg/n2TAtUoTztIa_mk2ldClsO0Vy_5dJuJgQCPcB/s1600/percabganan-di-repositori-git.png)

Sekarang setiap orang memiliki cabangnya masing-masing. Mereka bebas bereksperimen.

### Apa yang harus dilakukan apabila terjadi conflict?
You can resolve simple merge conflicts that involve competing line changes on GitHub, using the conflict editor.

You can only resolve merge conflicts on GitHub that are caused by competing line changes, such as when people make different changes to the same line of the same file on different branches in your Git repository. For all other types of merge conflicts, you must resolve the conflict locally on the command line. For more information, see "Resolving a merge conflict using the command line."

- Under your repository name, click  **Pull requests.**
![](https://docs.github.com/assets/images/help/repository/repo-tabs-pull-requests.png)
- In the "Pull Requests" list, click the pull request with a merge conflict that you'd like to resolve.
- Near the bottom of your pull request, click **Resolve conflicts.**
![](https://docs.github.com/assets/images/help/pull_requests/resolve-merge-conflicts-button.png)
- Decide if you want to keep only your branch's changes, keep only the other branch's changes, or make a brand new change, which may incorporate changes from both branches. Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge.
![](https://docs.github.com/assets/images/help/pull_requests/view-merge-conflict-with-markers.png)
- If you have more than one merge conflict in your file, scroll down to the next set of conflict markers and repeat steps four and five to resolve your merge conflict.
- Once you've resolved all the conflicts in the file, click **Mark as resolved.**
![](https://docs.github.com/assets/images/help/pull_requests/mark-as-resolved-button.png)
- If you have more than one file with a conflict, select the next file you want to edit on the left side of the page under "conflicting files" and repeat steps four through seven until you've resolved all of your pull request's merge conflicts.
![](https://docs.github.com/assets/images/help/pull_requests/resolve-merge-conflict-select-conflicting-file.png)
- Once you've resolved all your merge conflicts, click **Commit merge**. This merges the entire base branch into your head branch.
![](https://docs.github.com/assets/images/help/pull_requests/merge-conflict-commit-changes.png)
- If prompted, review the branch that you are committing to.

If the head branch is the default branch of the repository, you can choose either to update this branch with the changes you made to resolve the conflict, or to create a new branch and use this as the head branch of the pull request.
![](https://docs.github.com/assets/images/help/pull_requests/conflict-resolution-merge-dialog-box.png)
If you choose to create a new branch, enter a name for the branch.

If the head branch of your pull request is protected you must create a new branch. You won't get the option to update the protected branch.

Click **Create branch and update my pull request** or **I understand, continue updating** _BRANCH_. The button text corresponds to the action you are performing.
- To merge your pull request, click **Merge pull request**. For more information about other pull request merge options, see "Merging a pull request."
