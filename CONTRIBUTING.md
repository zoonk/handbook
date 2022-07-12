# Contributing to Zoonk

Thank you for your interest in contributing to Zoonk.
Please, make sure to read our [code of conduct](./CODE_OF_CONDUCT.md) and this entire page before you start.

## How we organize our tasks

Before we start, let's first understand [how we work](./how-we-work) and organize our tasks.
We value [transparency](./about/values.md#transparency) and [ownership](./about/values.md#ownership).
This means all our tasks are public.
Anyone can see what we're working on and encouraged to pick a task they'd like to work on.

The [project page](https://github.com/orgs/zoonk/projects/11) shows all the tasks that need to be done.
They're organized in the following manner:

|Board|Description|
|-----|-----------|
|Pending specs|Draft tasks. Someone needs to write the requirements for it.|
|Blocked|Tasks blocked by other tasks. After they're unblocked, move them to `Todo`.|
|Todo|Approved tasks. You can start working on them right away.|
|In Progress|Tasks that are actively being worked on. After you start working on a task, move it to this column.|
|In Review|Tasks that are partially finished and waiting for someone to review them. After you [open a pull request for a task](./how-we-work/how-to-use-github.md), move it to this column.|
|Done|Tasks that are completed and pushed to the `main` branch. It doesn't necessarily mean they're released to production yet.|

Issues that haven't been prioritized yet don't show up on the board.
You can see them by going to the [Backlog view](https://github.com/orgs/zoonk/projects/11/views/3).
To propose a new feature or report bugs, [start a discussion](./how-we-work/managing-discussions.md).

## Bugs, new features, brainstorming, and feedback

If you'd like to report a bug, suggest a feature, brainstorm ideas, or give us some feedback,
please [start a discussion](./how-we-work/managing-discussions.md) in the relevant project.
If you don't know what's the most appropriate project to start a discussion,
feel free to [start a discussion on the organization page](https://github.com/orgs/zoonk/discussions).
We'll redirect it to the appropriate project.

## How can I contribute to a Zoonk project?

- Go to the [project page](https://github.com/orgs/zoonk/projects/11).
- Choose an unassigned task from the `Todo` column.
- Assign the task to you.
- Move the task to `In Progress`.
- Create a new branch to work on your task.
- [Open a pull request](./how-we-work/how-to-use-github.md) after your work is done.
- Assign your pull request to the project lead (you can find them in the repository's README file).
- Move your task to the `In Review` column.

## Reviewing pull requests

After a pull request is reviewed, there are two outcomes possible:

### Pull request is approved

- **Reviewer:** After approving a `pull request`, publish the changes using the `squash and merge` option.
- **Automated:** The task moves from `In Review` to `Done`.

### Pull request is not approved

- **Reviewer:** Clearly state what changes need to be made (and why) for the work to be approved.
- **Reviewer:** Check the `Request changes` option. This will make the task go back to the `In Progress` column.
- **Reviewer:** Reassign the `pull request` to the author, so they can work on the requested changes.
- **Author:** Work on the requested changes (or comment why you don't agree with them) until the `pull request` is approved.

### Merging pull requests

- Use the `Squash and merge` option to merge a pull request.
- Make sure to remove all the commits from the description before merging a pull request to keep the history clean.

## Creating tasks

Follow the steps below to create a new task:

- [ ] Go to the [`All` tab of this project's task management tool](https://github.com/orgs/zoonk/projects/11/views/2).
- [ ] Use `Ctrl + Spacebar` to create a new item.
- [ ] Select the newly created item, click on the down arrow, then click on the `Convert to issue` button:

![GitHub screenshot showing how to convert an item into an issue](https://user-images.githubusercontent.com/4393133/178562514-e66903ec-ed0e-4998-a679-2d6dbeee9cc1.png)

- [ ] Select the repository where you'd like to create this task.
      If it's an `Epic` (it has sub-tasks) and it belongs to multiple repositories, then select `.github`.
- [ ] In the `Status` column, select one of the options according to the [`How we organize our tasks` table above](#how-we-organize-our-tasks).
- [ ] In the `Category` column, select `Epic` if it will have sub-tasks.
      Otherwise, select `Bug` for issues, `Feature` for new functionality, or `Enhancement` for improvements to existing functionality.
- [ ] In the `Asignees` column, select who is going to work on this task (or leave it empty if you don't know yet).
      If it's an `Epic`, then assign yourself because it's your responsability to ensure all tasks are completed.
