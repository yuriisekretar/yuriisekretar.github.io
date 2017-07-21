Project management is not always simple task for a software developer. Developers used to a solutions built for them. But if such tool can combine hosting and reviewing code, managing projects, and building software in a teams - it will make road to successful project easier.

Integrated project management was introduced by GitHub and basic functionality covered in the [GitHub documentation](https://help.github.com/categories/managing-your-work-on-github/). However, there are few tricks  I use to organize my work between multiple organizations and repositories.

## Adding an email address to your account

When you are working on multiple projects or invited in a team it is easier to use one username for all of them. But it's a good practice to use different emails. Using GitHub Settings just add additional email that you will use in your commits.
![github-email](/public/posts/github-email.png)
Do not forget to use your username in combination with required email in your future commits for the specific repository.

### Example using git in command line:

```bash
git config user.email "email@example.com"
```

Now everytime you commit it will display correct username and email.

## Scheduling releases and organizing versions in project
 
Versions are very important points-in-time for a project. They help you schedule and organize your releases and your users expect new features or improvements with every new version. 

Repository project boards are scoped to issues, pull requests, and notes within a single repository and they can be used for scheduling releases and organizing versions for current repository.

To create a version I simply add new Project with a name corresponding to the version, e.g. `v1.56`. I use Description to add details about new features or improvements current version will have. By the way, same text could be used while creating release for a repository. 
![github-project](/public/posts/github-project.png)

Once a version is created and issues are assigned to it, use Project columns to organize your workflow. Great introduction to Projects you can read at [GitHub blog](https://github.com/blog/2256-a-whole-new-github-universe-announcing-new-tools-forums-and-features).

## Discipline in a team with Milestones

In my practice for each GitHub repository there is dedicated small team and often people are working remotely. It is important for everybody keep focus during development.

I organize Milestones around small amount of tasks and limit them to one-two weeks. [GitHub Milestones](https://help.github.com/articles/about-milestones/) have all features needed to better manage your project like list of issues, due date and completion percentage. These parameters are very handy during team meetups that take place on a due date of Milestone. 
![github-milestone](/public/posts/github-milestone.png)

Milestones like Sprints help project members communicate more effectively especially when working together remotely.

As a result these simple adaptation of GitHub features helps me build software easier and ship high-quality code.
