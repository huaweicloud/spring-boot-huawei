# How to contribute

This project is [Apache 2.0](LICENSE) licensed and accepts contributions via GitHub pull requests. This document outlines some of the conventions on commit message formatting, contact points for developers and other resources to make getting your contribution easier.

Before you start, NOTICE that ```main``` branch is the relatively stable version
provided for customers and users. So all code modifications SHOULD be submitted to
```development``` branch.

## Report issues

A great way to contribute to the project is to send a detailed report when you encounter an issue. We always appreciate a well-written, thorough bug report and feature propose, and will thank you for it!

### Issues format

When reporting issues, refer to this format:

- Is this a BUG REPORT or FEATURE REQUEST?
- What happened?
- What you expected to happen?
- What happened?
- How to reproduce it (as minimally and precisely as possible)
- Anything else we need to know?
- Environment

See more about [ISSUE_TEMPLATE](.github/ISSUE_TEMPLATE.md).

## Submit pull requests

If you are a beginner and expect this project as the gate to open source world, this tutorial is one of the best
choices for you. Just follow the guidance and you will find the pleasure to becoming a contributor.

### Step 1: Fork repository

Before making modifications of this project, you need to make sure that this project have been forked to your own
repository. It means that there will be parallel development between this repo and your own repo, so be careful
to avoid the inconsistency between these two repos.

### Step 2: Clone the remote repository

If you want to download the code to the local machine, ```git``` is the best way:
```
git clone https://github.com/huaweicloud/spring-boot-huawei.git
```

### Step 3: Develop code locally

To avoid inconsistency between multiple branches, we SUGGEST checking out to a new branch:
```
git checkout -b new_branch_name origin/devlopment
```
Then you can change the code arbitrarily.

### Step 4: Push the code to the remote repository

After updating the code, you should push the update in the formal way:
```
git add .
git status (Check the update status)
git commit -m "Your commit title"
git commit --amend (Add the concrete description of your commit)
git push origin new_branch_name
```

### Step 5: Pull a request to repository

In the last step, your need to pull a compare request between your new branch and development branch. After
finishing the pull request, the travis CI will be automatically set up for building test.

### Pull requests format

When submitting pull requests, refer to this format:

- What this PR does / why we need it?
- Which issue this PR fixes?
- Special notes for your reviewer
- Release note

See more about [PULL_REQUEST_TEMPLATE](.github/PULL_REQUEST_TEMPLATE.md).

### Code style

The coding style suggested by the Golang community is used. See the [doc](https://github.com/golang/go/wiki/CodeReviewComments) for more details.

Please follow this style to make it easy to review, maintain and develop.
