# How we manage projects

We use GitHub to manage our projects and tasks.
The [projects page](https://github.com/orgs/zoonk/projects?type=beta) lists all activities we're currently working on.
All projects have tasks that need to be done.
We value [ownership](../about/values.md#ownership).
Therefore, it's up to us to pick a project or task we'd like to work on.
We don't expect others to tell us what to do.
Make sure to read the [contributing guide](../CONTRIBUTING.md) to understand how to get started.

## How to start a project

When starting a new project, there are two things you need to do:

### 1. Create a new project

Every project should be visible at the [projects page](https://github.com/orgs/zoonk/projects?type=beta).
It doesn't matter if it's working in progress.
Everything is always in progress. :)
We build in public and building in public means we start sharing things as soon as we start working on them.

Do the following steps to create a new project:

- [ ] Go to the [projects page](https://github.com/orgs/zoonk/projects?type=beta).
- [ ] Click on the `New project` button.
- [ ] Choose the `Board` template and click on `Create`.
- [ ] Give a name to your project by clicking on the `@myusername's untitled project` title and changing it.
- [ ] Rename `View 1` to `Kanban` by clicking on it.
- [ ] After the last column, click on the `+` add to add a new column.
- [ ] Name the new column `Backlog`. We'll keep all unprioritized tasks there.
- [ ] Drag the `Backlog` column to the start, so it becomes the first column.
- [ ] Create a new column and call it `In Review`. We'll add tasks with open pull requests here.
- [ ] Move the `In Review` column between `In Progress` and `Done`.
- [ ] Create a new view by clicking on the `New view` button.
- [ ] Use the `Table` format for the new view.
- [ ] Rename this new view to `Tasks`.
- [ ] Edit the project settings by clicking on the `...` button, then `Settings`.
- [ ] Add a brief description explaining what's the goal of your project.
- [ ] Click on the `Save` button to save your description.
- [ ] Scroll down to the `Danger zone` area.
- [ ] Under `Visibility`, change it from `Private` to `Public`.
- [ ] On the left sidebar, go to the `Manage access` menu.
- [ ] Under `Invite collaborators`, add the team responsible for managing this project.
- [ ] Select the `Write` role.
- [ ] Click on `Invite` to invite them to join the project.

### 2. Create a new repository

All information about your project will live in a repository.
Therefore, you need to create a repository for your project now:

- [ ] Navigate to the [repositories page](https://github.com/orgs/zoonk/repositories) for the Zoonk organization.
- [ ] Click on the `New repository` button.
- [ ] Select `zoonk` as the `Owner`.
- [ ] Give a name to the repository under `Repository name`.
It should be the same or a short version of the project name.
If you have space between words, then separate words using `-` (i.e. `my-fancy-new-project`).
- [ ] Give a brief description to your project.
- [ ] Select the `Public` option. As mentioned earlier, we value [transparency](../values.md#transparency) and we build in public.
- [ ] Check the `Add a README file` option.
- [ ] Under `Choose a license`, select `MIT` for software projects or `Creative Commons Zero v1.0 Universal` for content projects.
- [ ] Click on the `Create repository` button.

After the repository is created, let's add some default configurations.
We can start by adding our code of conduct to your repository.

- [ ] Go to your new repository.
- [ ] Click on the `Insights` tab.
- [ ] Click on the `Community Standards` menu.
- [ ] Under `Code of conduct`, click the `Add` button.
- [ ] Select the `Contributor Covenant` option.
- [ ] Under `Contact method`, type `https://forms.gle/48UjFHCFByxCfd12A`.
- [ ] Click on the `Review and submit` button.
- [ ] Under `Commit new file`, select the `Commit directly to the `main` branch option.
- [ ] Click on the `Commit new file` button.

We use GitHub Discussions to report bugs, suggest new features, and brainstorm ideas.
Therefore, Issues should only be created by our own team.
To avoid having external contributors creating issues without a discussion first, we need to update our issue templates:

- [ ] Create a new file under `.github/ISSUE_TEMPLATE` called `config.yml`
- [ ] Copy [this content](../.github/ISSUE_TEMPLATE/config.yml) into the new file.
- [ ] Update the links in the file to use your new repository's URL.
- [ ] Create a new file under `.github/ISSUE_TEMPLATE` called `approved-task.md`.
- [ ] Copy [this content](../.github/ISSUE_TEMPLATE/approved-task.md) into the new file.

Now, let's update the general configurations for our repository:

- [ ] Go to the `Settings` tab of your repository.
- [ ] Update the social preview image.
Make sure to update the preview available in our [social-media repository](https://github.com/zoonk/social-media)
to include your repository name.
If you don't know how to edit the preview file, create a new issue in that repository asking for a designer to do it for you.
- [ ] Under `Features`, disable the `Wiki` option.
- [ ] Enable the `Issues` option.
- [ ] Enable the `Projects` option.
- [ ] Enable the `Preserve this repository` option.
- [ ] Enable the `Discussions` option.
- [ ] Under `Pull Requests`, disable the `Allow merge commits` option.
- [ ] Enable the `Allow squash merging` option.
- [ ] Enable the `Default to PR title for squash merge commits` option.
- [ ] Disable the `Allow rebase merging` option.
- [ ] Enable the `Always suggest updating pull request branches` option.
- [ ] Enable the `Automatically delete head branches` option.

Our next step is to update the `Collaborators and teams` configurations:

- [ ] In the `Settings` page, click on the `Collaborators and teams` menu on the left sidebar.
- [ ] Under `Manage access`, click on the `Add teams` button.
- [ ] Search the team that should have access to this repository (or [create a new team](https://github.com/orgs/zoonk/new-team) first).
- [ ] Select the `Maintain` option for your team.

Let's update the moderation options now:

- [ ] In the `Settings` page, click on the `Moderation options` menu on the left sidebar:
- [ ] Go to the `Code review limits` page.
- [ ] Enable the `Limit to users explicitly granted read or higher access` option.

After updating our moderation options, we need to change our branches settings:

- [ ] In the `Settings` page, find the `Code and automation` section and click on the `Branches` menu.
- [ ] Under `Branch protection rules`, click on the `Add rule` button.
- [ ] In `Branch name pattern`, type `main` to match the `main` branch.
- [ ] Scroll down to `Protect matching branches`.
- [ ] Enable the `Require a pull request before merging` option.
- [ ] Enable the `Require approvals` option.
- [ ] Select `1` in the `Required number of approvals before merging` option.
- [ ] Enable the `Dismiss stale pull request approvals when new commits are pushed` option.
- [ ] Enable the `Allow specific actors to bypass required pull requests` option.
- [ ] Enable the `Require status checks to pass before merging` option.
- [ ] Enable the `Require branches to be up to date before merging` option.
- [ ] Enable the `Require conversation resolution before merging` option.
- [ ] Enable the `Require linear history` option.
- [ ] Enable the `Require deployments to succeed before merging` option.
- [ ] Disable the `Allow force pushes` option.
- [ ] Disable the `Allow deletions` option.
- [ ] Click on the `Create` button.

If you're creating a non-software repository, you likely don't need [GitHub Actions](https://github.com/features/actions).
If that's the case, make sure to disable it:

- [ ] In the `Settings` page, find the `Actions` section and click on the `General` menu.
- [ ] Select the `Disable actions` option.
- [ ] Click on the `Save` button.

If you're creating a software repository,
make sure to review the security options (`Security` tab)
and the community standards (`Insights` tab -> `Community Standards` menu).

Clean up unused features:

- [ ] Navigate to the `Code` tab of your repository.
- [ ] Under `About` click on the `clog` (settings) icon.
- [ ] Add relevants tags to your project (i.e. `handbook`, `management`, `design`, etc.).
- [ ] Uncheck all the options you won't use (i.e. non-software projects probably won't use `releases`, `packages`, and `environments`).

Now, you need to link this repository to the project you previously created:

- [ ] Go to your new repository.
- [ ] Click on the `Projects` tab.
- [ ] Click on the `Add project` button.
- [ ] Select the project you've created.

## Found an issue?

- [Suggest a change](https://github.com/zoonk/handbook/edit/main/how-we-work/managing-projects.md)
- [Start a discussion](https://github.com/zoonk/handbook/discussions/new)
