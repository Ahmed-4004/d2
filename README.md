to delete locally : git branch -d <branch-name>
to delete remotly : git push origin --delete <branch-name>
<img src="images/tree-736885_1280.jpg" width="300" alt="image">

Annotated Tags vs Lightweight Tags
Annotated Tags
Metadata: They store additional metadata, such as the tagger's name, email, and date, along with a message (like a commit message).
Commit Object: An annotated tag creates an extra Git object in the repository.
Verification: They can be GPG-signed for verification purposes, making them ideal for release tags.
Use Case: Best for tagging important milestones (like version releases) where detailed information and verification are required.

Lightweight Tags
Simplicity: They are just pointers to commits and lack the metadata that annotated tags have.
Commit Object: No additional Git object is created; it's essentially a named reference to a commit.
Use Case: Ideal for quick, temporary tagging or less critical use cases where metadata isn't necessary.

we use rebase :- 
1- Keep a linear history: It rewrites commit history, making it cleaner and easier to understand.
2- Integrate changes: Apply commits from one branch onto another, like keeping feature branches updated with the latest   changes from the main branch.
3- Avoid merge commits: Instead of creating a merge commit, rebase applies changes directly onto the base branch.

- we list tags by : git tag

- we delete tag locally : git tag -d <tag-name>
- we delete tag remotly : git push origin --d <tag-name>