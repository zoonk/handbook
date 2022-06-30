# Contributing to Zoonk

Thank you for your interest in contributing to Zoonk.
Please, make sure to read our [code of conduct](./CODE_OF_CONDUCT.md) and this entire page before you start.

## How we organize our tasks

Before we start, let's first understand [how we work](./how-we-work) and organize our tasks.
We value [transparency](../about/values.md#transparency) and [ownership](../about/values.md#ownership).
This means all our tasks are public.
Anyone can see what we're working on and encouraged to pick a task they'd like to work on.

The [projects page](https://github.com/orgs/zoonk/projects?type=beta) shows all the tasks that need to be done for each project.
They're organized in the following manner:

|Board|Description|
|-----|-----------|
|Todo|Approved tasks. You can start working on them right away.|
|In Progress|Tasks that are actively being worked on. After you start working on a task, move it to this column.|
|In Review|Tasks that are partially finished and waiting for someone to review them. After you [open a pull request for a task](./how-we-work/how-to-use-github.md), move it to this column.|
|Done|Tasks that are completed and pushed to the `main` branch. It doesn't necessarily mean it's released to production yet.|

Issues that haven't been prioritized yet don't show up on the board.
You can see them by going to the `Backlog` view.
To propose a new feature or report bugs, [start a discussion](./managing-discussions.md).

## Bugs, new features, brainstorming, and feedback

If you'd like to report a bug, suggest a feature, brainstorm ideas, or give us some feedback,
please [start a discussion](./how-we-work/managing-discussions.md) in the relevant project.
If you don't know what's the most appropriate project to start a discussion,
feel free to [start a discussion on the organization page](https://github.com/orgs/zoonk/discussions).
We'll redirect it to the appropriate project.

## How can I contribute to a Zoonk project?

- [Pick a project](https://github.com/orgs/zoonk/projects?type=beta) you'd like to work on.
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

- The reviewer should merge the changes using the "stash and merge" option.
- The reviewer should move the task from `In Review` to `Done` (if that wasn't done automatically).

### Pull request is not approved

- The reviewer should clearly state what changes are required (and why) to merge that work.
- The reviewer should reassign the pull request to the author, so they can work on the requested changes.
- The reviewer should move the task from `In Review` to `In Progress`.
- The author should work again on the required changes until their work is approved.

### Merging pull requests

- Use the `Squash and merge` option to merge a pull request.
- Make sure to remove all the commits from the description before merging a pull request to keep the history clean.
