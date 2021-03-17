[The GitHub pages documentation](https://pages.github.com/)


![create a_repo](/images/003/create_a_repo.png)

![switch branch](/images/003/switch_branch.png)

![go to_settings](/images/003/go_to_settings.png)

![create pages](/images/003/create_pages.png)

![choose a_theme](/images/003/choose_a_theme.png)

![commit pages](/images/003/commit_pages.png)

![setup pages](/images/003/setup_pages.png)

![hosted page](/images/003/hosted_page.png)



![clone_the_repo](/images/003/clone_the_repo.png)

```bash
[12:13] Blog $  : git clone git@github.com:AEJaspan/make-a-blog.git
```
```text
Cloning into 'make-a-blog'...
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 8 (delta 1), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (8/8), done.
Resolving deltas: 100% (1/1), done.
```

```bash
[12:13] Blog $  : cd make-a-blog/
[12:13] make-a-blog $  : git branch -a
```

```text
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/gh-pages
  remotes/origin/main
```

```bash
[12:13] make-a-blog $  : git checkout remotes/origin/gh-pages
```

```text
Note: switching to 'remotes/origin/gh-pages'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 61a3cbe Create index.md
```

```bash
[12:14] make-a-blog $  : git branch -a
```

```text
* (HEAD detached at origin/gh-pages)
  main
  remotes/origin/HEAD -> origin/main
  remotes/origin/gh-pages
  remotes/origin/main
```

```bash
[12:14] make-a-blog $  : git switch gh-pages
```

```text
Branch 'gh-pages' set up to track remote branch 'gh-pages' from 'origin'.
Switched to a new branch 'gh-pages'
```

```bash
[12:14] make-a-blog $  : git branch -a
```

```text
* gh-pages
  main

  remotes/origin/HEAD -> origin/main
  remotes/origin/gh-pages
  remotes/origin/main
```

```bash
[12:15] make-a-blog $  : git switch main
```

```text
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

```bash
[12:15] make-a-blog $  : git branch -a
```

```text
  gh-pages
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/gh-pages
  remotes/origin/main
```


```bash
[12:24] make-a-blog $  : git switch gh-pages
```

```text
Switched to branch 'gh-pages'
Your branch is up to date with 'origin/gh-pages'.
```

```bash
[12:24] make-a-blog $  : mkdir -p BlogPosts/Post001
[12:25] make-a-blog $  : echo '# My first blog post!' > BlogPosts/Post001/index.md
[12:26] make-a-blog $  : echo '[link to post](BlogPosts/Post001/index.md)' > index.md
[12:27] make-a-blog $  : git add index.md
[12:27] make-a-blog $  : git add BlogPosts/
[12:27] make-a-blog $  : git commit -m 'Creating my first blog post!'
```

```text
[gh-pages 9809b7d] Creating my first blog post!
 2 files changed, 2 insertions(+), 37 deletions(-)
 create mode 100644 BlogPosts/Post001/index.md
 rewrite index.md (100%)
```

```bash
[12:27] make-a-blog $  : git push
```

```text
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 494 bytes | 494.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:AEJaspan/make-a-blog.git
   61a3cbe..9809b7d  gh-pages -> gh-pages
```

![landing_page](/images/003/landing_page.png)

![first_post](/images/003/first_post.png)
