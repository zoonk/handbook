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

We're using GitHub because we think it's the easiest way to open-source everything we do,
keep our processes transparent, organize our conversations, and do all that asynchronously in one place.

We're not saying GitHub is perfect.
There are more feature-complete tools for task management and discussions.
However, every choice comes with trade-offs.
At the moment, we believe having all information about us in one place (GitHub)
helps us to reach our goals and it's more aligned with our values (../about/values.md),
especially the transparency one.
It would be harder to reach the same level of transparency and eficiency using multiple tools
because it would increase this project's complexity and [our resources are limited](https://github.com/zoonk/finances).

## Core concepts

- **Projects:** Where we manage our tasks.
- **Repositories:** Where we keep our project files.
- **Issues:** Tasks we need to work on.
- **Branch:** A folder where we temporarily keep changes we're making.
- **Pull request**: A request to publish our changes to the `main` branch.
- **Discussions:** A forum where we keep all conversations and decisions about a project.

## How to make changes

This guide will focus on making changes using the github.com website.
However, you can also use the following options for more advanced use cases (not mandatory):

- [GitHub Desktop](https://desktop.github.com/)
- [GitHub CLI](https://cli.github.com/)
- [Git CLI](https://github.com/git-guides/install-git)
- [VS Code](https://code.visualstudio.com/)
- [GitHub Codespaces](https://github.com/features/codespaces)

### Creating a branch

The first thing you need to do when working on a task is to [create a new branch](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/managing-branches).
It's useful if you have a descriptive branch name, including your username and the task ID (i.e. `myusername/23-update-github-guide`).

### Update a file

After you've created your branch, navigate to the file you'd like to update.
For example, this one is located in `how-we-work` -> `how-to-use-github.md`.

GitHub has a pencil icon to edit a page. Click on it and select the `Edit this file` option:

<img alt="GitHub screenshot showing the 'edit this file' option" src="https://user-images.githubusercontent.com/4393133/175760174-2da05369-b088-43e5-abc7-5070efa32f4a.png">

GitHub will open a text editor with the file content.
Make all the changes you need.
The editor is using the [Markdown format](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

After you finish editing your file, click on the `Commit changes` button to save your changes:

<img alt="GitHub screenshot showing the commit changes option" src="https://user-images.githubusercontent.com/4393133/175760264-4386974a-eb66-4827-a981-a2fe0f3b47df.png">

Those changes are saved in your branch only.
They haven't been published to the `main` branch yet.
If you need to edit more files, follow the same steps above.
Otherwise, skip to the [Publishing your changes](#publishing-your-changes) section below.

### Add files

Before adding your file, make sure you've [created a new branch](#creating-a-branch)
for your changes and that you're working on that branch instead of `main`.

After your branch is created, you can add a new file by clicking on the `Add file` -> `Create new file` button.
If you have those files on your computer, you can use the `Upload files` option instead.

<img alt="GitHub screenshot showing the create file option" src="https://user-images.githubusercontent.com/4393133/175760441-23dbdf2b-71af-4020-b9ce-7fc79571436d.png">

Before you add any content to your file, make sure to give it a name:

<img alt="GitHub screenshot showing the new file name input" src="https://user-images.githubusercontent.com/4393133/175760469-2a4c19c0-4371-4ac5-abc7-c8566170863d.png">

You can add that file to a specific folder by typing `/` after the folder name.
For example, `about/values/README.md` would create a `README.md` file in the `about/values` folder.
If either `about` or `values` don't exist, then GitHub will create that folder for us.

After you name your file, add the desired content and click on the `Commit changes` button to save your new file.
Again, this file will be saved to your branch only.
You still need to [send a request to publish your changes](#publishing-your-changes).

### Delete a file

For deleting a file, you need to follow the same steps you did for updating a file.
However, you'll need to click on the `trash` icon instead of clicking on the `pencil` one.

### Publishing your changes

As we mentioned in the [core concepts section](#core-concepts), a `branch` is the place where we temporalily save your changes.
Right now, your changes are visible only in the branch you created. They're not published yet.
It's like a draft. We can put anything there. It won't affect the `main` branch.
To publish your changes to the `main` branch, you need to open a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

A pull request is how you ask someone to review your changes.
After your change is approved, it will published to the `main` branch and your temporary branch will be deleted.
To open a pull request you can do the following:

- Click on the `Pull requests` tab.
- Click on the `New pull request` button.
- In the `base` menu, select the `main` branch. That's where you need to publish your changes.
- In the `compare` menu, select the branch name you're currently working on.
- Click on the `Create pull request` button.

GitHub will show you all changes you made. Please, review them before opening your pull request.
If everything is correct, do the following steps:

- Add a descriptive title for your changes, starting with the section you're updating (i.e. `How we work: Update instructions for deleting a file`).
- Describe the changes you made and add any comments that may be relevant to explain your changes.
- If your pull request is related to a task, make sure to use the keyword `Closes #42` where `42` is the task ID.
This will close that task once your pull request is published to `main`.
- On the right side, you'll side the `Reviewers` and `Assignees` items:

<img alt="GitHub screenshot showing a pull request sidebar menu" src="https://user-images.githubusercontent.com/4393133/175761006-966d6a5c-b91e-49fe-bf07-0520e223974e.png">

Make sure to ask a review from the project lead and assign this pull request to them as well.
You can find the project lead in the main `README.md` file.

Now, click on the "Create pull request" button.
Your pull request will be created.
After it's approved, the reviewer will publish it to the `main` branch.

**Important:** After you create a pull request, please make sure to move your task from `In Progress` to `In Review`.
If you're making a small change (i.e. fixing a typo), you don't need to create a task for it.
