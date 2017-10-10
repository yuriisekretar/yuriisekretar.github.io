---
layout: post
title: "How to Manage Projects on GitHub"
---

Project management is not always a simple task for a team lead. The market offers a lot of solutions built for managers, not for software developers. But what if those solutions could combine hosting and reviewing code, managing projects, tools for building software in teams?

One of such solutions called Integrated Project Management was introduced by GitHub and its basic functionality is covered in the [GitHub documentation](https://help.github.com/categories/managing-your-work-on-github/).

Here are some ideas on how I organize my work between multiple organizations and repositories.

## Adding an email address to your account

Either you are working on multiple projects or you are a member of a team, it is easier to use one single account. But it is a good practice to use different emails. Using GitHub Settings simply add an additional email that you will be using in your commits.

![github-email](/public/posts/github-email.png)

Do not forget to use your username in combination with required email in your future commits for the specific repository.

### Example using git in command line:

```bash
git config user.email "email@example.com"
```

From now on, every time you commit, it will display the correct username and email.

## Scheduling releases and organizing versions in a project

Versions are very important points-in-time for a project. They help you schedule and organize your releases, and your users expect new features or improvements with every new version.

Repository project boards are scoped to issues, pull requests, and notes within a single repository and they can be used for scheduling releases and organizing versions for current repository.

In order to create a version, I simply add new Project with a name corresponding to the version, e.g. v1.56. I use Description to add details about new features or improvements that a current version will have. By the way, the same text could be used while creating a release for a repository.

![github-project](/public/posts/github-project.png)

Once a version is created and issues are assigned to it, use Project columns to organize your workflow. You can find an Introduction to Projects at [GitHub blog](https://github.com/blog/2256-a-whole-new-github-universe-announcing-new-tools-forums-and-features).

## Setting discipline in a team with Milestones

It is important that everybody in a team stays focused especially if working remotely. I use Milestones for this purpose. Usually, there is a dedicated small team for each GitHub repository. I set up Milestones for several tasks and limit them to one-two weeks. [GitHub Milestones](https://help.github.com/articles/about-milestones/) have all features needed to manage your projects better, i.e. a list of issues, due date, and completion percentage. These parameters are very handy at team meetings on a due date of Milestone.

![github-milestone](/public/posts/github-milestone.png)

Milestones like Sprints help project members communicate more effectively.

By leveraging GitHub Integrated Project Management features, my teams build software more effectively and ship high-quality code.
