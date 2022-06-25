# How to use GitHub

This guide is focused on non-coders because there are plenty of Git learning resources online for developers.
Regardless if you're a junior software engineer or a non-coder, you also recommend you to read [GitHub's hello world tutorial](https://docs.github.com/en/get-started/quickstart/hello-world) and their [Git Guide](https://github.com/git-guides/install-git).
The US government website also has a [guide on how GitHub works](https://digital.gov/resources/an-introduction-github/).
Here, we'll focus on how we can use GitHub for managing our work at Zoonk.

## What is Git?

Git is a tool for managing different versions of files.
For example, instead of having `my_file_v1`, `my_file_v2`, etc., we have only one file and we can check its history change using Git.

## What is GitHub?

GitHub is a website that allows us to use Git in a friendly way.

## What's the difference between Git and GitHub?

Git is the technology that allows version control. GitHub is a service that uses that technology.
They're commonly used in software engineering.
But, here at Zoonk, we're also using them for documentation and managing our processes.

## Why we use GitHub

We're using GitHub because we think it's the easiest to open-source everything we do,
keep our processes transparent, organize our conversations, and do all that asynchronously in one place.

## Core concepts

- **Projects:** Where we manage our tasks.
- **Repositories:** Where we keep our project files.
- **Issues:** Tasks we need to work on.
- **Branch:** A folder where we temporarily keep changes we're making.
- **Pull request**: A request to publish our changes to the `main` branch.
- **Discussions:** A forum where we keep all conversations and decisions about a project.

## How to make changes

This guide will focus on making changes using the github.com website.
However, you can also use the following options for more advanced use cases:

- [GitHub Desktop](https://desktop.github.com/)
- [GitHub CLI](https://cli.github.com/)
- [Git CLI](https://github.com/git-guides/install-git)
- [VS Code](https://code.visualstudio.com/)
- [GitHub Codespaces](https://github.com/features/codespaces)

### Creating a branch

The first thing you need to do when working on a task is to [create a new branch](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/managing-branches).
It's useful if you have a descriptive branch name, including your name and the task ID (i.e. `myusername/23-update-github-guide`).

### Update a file

After you've created your branch, navigate to the file you'd like to update.
For example, this one is located in `how-we-work` -> `how-to-use-github.md`.

GitHub has a pencil icon to edit a page. Click on it and select the `Edit this file` option:

<img alt="GitHub screenshot showing the 'edit this file' option" src="https://user-images.githubusercontent.com/4393133/175760174-2da05369-b088-43e5-abc7-5070efa32f4a.png">

GitHub will open a text editor with the file content.
Make all the changes you need.
The editor is using the [Markdown format](https://www.markdownguide.org/getting-started/).

After you finish editing your file, click on the `Commit changes` button to save your changes:

<img alt="GitHub screenshot showing the commit changes option" src="https://user-images.githubusercontent.com/4393133/175760264-4386974a-eb66-4827-a981-a2fe0f3b47df.png">

Those changes are saved in your branch only.
They haven't been published to the `main` branch yet.
If you need to edit more files, follow the same steps above.
Otherwise, skip to the [Publishing your changes](#publishing-your-changes) section below.

### Add files

### Delete a file

### Publishing your changes

## Found an issue?

- [Suggest a change](https://github.com/zoonk/handbook/edit/main/how-we-work/how-to-use-github.md)
- [Start a discussion](https://github.com/zoonk/handbook/discussions/new)
