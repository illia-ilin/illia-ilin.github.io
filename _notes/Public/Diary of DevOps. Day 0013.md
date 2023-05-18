---
title: Diary of DevOps. Day 0013
feed: show
date: 16-05-2023
permalink: /diary-of-devops-day-0013
---

According to the [[ChatGPT's 30 Days of DevOps]], the fifth day plan is:

#### **Day 5: Version Control**
- Read: [Git Branching and Merging Strategies](https://www.atlassian.com/git/tutorials/comparing-workflows)
- Practice: [Create a GitHub repository and practice different Git workflows](https://guides.github.com/introduction/git-handbook/)

I've decided to recap some Git things with Online [Learn Git Branching](https://learngitbranching.js.org/) service.

The very first exercise may not work, so in case something doesn't work properly, it's better to check [issues](https://github.com/pcottle/learnGitBranching/issues) at their repository.

```bash
# Detach yo' HEAD
git checkout C4

# Level Relative Refs (^)
git checkout bugFix^

# Level Relative Refs (~)
git branch -f main C6
git checkout HEAD^
git branch -f bugFix HEAD^

# Level Reversing Changes in Git
git reset HEAD^
git checkout pushed
git revert HEAD^

# Level Cherry-pick Intro
git cherry-pick C3 C4 C7

# Level Interactive Rebase Intro
git rebase -i HEAD~4

# Level Grabbing Just 1 Commit
git checkout main
git cherry-pick C4

# Level Juggling Commits
git rebase -i HEAD~2
git commit --amend
git rebase -i HEAD~2
git rebase caption main

# Level Git Tags
git checkout C2
git tag v1
git tag v0 C1

# Level Git Describe
git describe bugFix
git describe side
git commit

# Level Rebasing over 9000 times
git rebase main bugFix
git rebase bugFix side
git rebase side another
git rebase another main

# Level Multiple parents
git branch bugWork HEAD^^2^

# Level Branch Spaghetti
git checkout one
git cherry-pick C4 C3 C2
git checkout two
git cherry-pick C5 C4 C3 C2
git branch -f three C2

# Level Clone Intro
git clone



```

Another good service is [GitHub Minesweeper](https://profy.dev/project/github-minesweeper) - it offers a plenty of practical things to do with git and GitHub - commits, pull requests, and so on.

#### Documenting the time I spend

Today I created a Google Sheet to document time I am spending during a day. [This is the copy to use](https://docs.google.com/spreadsheets/d/1S6Di6Btsbt9rrH9lckotn6tg2JrWahemhkmZ9XwO9n0/edit?usp=sharing).
There are 15-minutes blocks of time and dropdown lists.
It's nice for analyzing habits. In addition to the Toggl app I am using for particular blocks of time.

#### Current progress

Task | Type | Progress
--- | --- | ---:
"The Phoenix Project" | book | 4/35 chapters, 14%
"The DevOps Handbook" | book | 9%
AWS Cloud Quest | course | 7/12 assigments, 58%

Tags: #Git