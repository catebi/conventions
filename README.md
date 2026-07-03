# Conventions
Our conventions about development principles and tech stack. Read it first before starting to work on any project!

## Tech Stack

We stick to the same tech stack for all our projects. This allows us to easily replace each other and switch between projects.

Of course, there are cases when something different would be a better choice. In those cases, please discuss it with the other developers and explain why it would be a better choice. If we agree, please provide information on how to work with the tool / library so that others can learn it and participate in the development process.

Most of our projects are Telegram bots. We use this stack:

- Python 3.12+
- PyTelegram for interaction with Telegram API
- FastAPI + Uvicorn as a server
- Asyncio + APScheduler for thread and tasks manipulations
- Pydantic for data models and settings
- PyAirtable + Ngrok for interaction with Airtable API and webhooks
- PostgreSQL as DB
- Docker + Docker Compose for deployment
- GetText built in module to provide localizations

Some old projects need to be refactored and migrated to the current stack. Help is appreciated ;)

Our API is currently in C#, we're working on API V2, which will be written in Python.

Tech stack for frontend projects: TBA

## Core Principles

1. Avoid vibe coding. We have lots of problems that need to be solved ASAP, and that's exactly why. We have experienced developers on our team, so you can ask them to do something or ask them to teach you something new. Instead of trying to save time with AI tools, let's help each other grow. Actually, they've been proven to actually increase development time and effort.
2. If you're starting a new project, discuss it with the volunteers who will benefit from it. This way, you can create an intuitive and helpful tool that considers the users needs.
3. Write proper documentation. Other developers should be able to easily understand how to maintain your project, even if you're unavailable. The same goes for explaining to volunteers how to use your project. Most of them aren't developers, so your instructions should be clear even without specific technical knowledge. Therefore, a good README is a must. Additionally, we keep our guides on Notion and, in the near future, on Google Workspace.
4. Make the development process transparent by starting with a GitHub repository and steadily adding commits instead of uploading an entire new project that no one has seen before. This will make it much easier to review.
5. Don't forget to use the repository issues tab to track the issues and features. This helps us stay on the same page, even if others don't maintain this project. It also helps if you haven't worked on the repository in a while.
6. Make your commits granular. It is better to divide one big task into several smaller ones and create a merge request for each task. Even if it's a single task, you can do it as a single PR with multiple commits - that way, it will be easier to review per-commit
7. It's totally OK to ask developers who aren't maintaining this project to be the reviewers. They may notice things that you haven't because you've been working on this project for so long.
8. Don't merge anything without at least one approval. If nobody has reviewed the MR yet, don't be shy about pinging others in the IT topic. Sometimes, we may overlook or forget to check it.
9. Avoid merge conflicts whenever possible. There is usually no need to work on several tasks that affect the same things at once. Wait to merge an MR with the main branch first. This process won't take much time, but it will make the Git history clear and easy to read.
