---
title: Getting Started
description: >-
  Get started with Chirpy basics in this comprehensive overview.
  You will learn how to install, configure, and use your first Chirpy-based website, as well as deploy it to a web server.
author: cotes
date: 2019-08-09 20:55:00 +0800
categories: [Blogging, Tutorial]
tags: [getting started]
pin: true
---

## Creating a Site Repository

When creating your site repository, you have two options depending on your needs:

### Option 1. Using the Starter (Recommended)

This approach simplifies upgrades, isolates unnecessary files, and is perfect for users who want to focus on writing with minimal configuration.

1. Sign in to GitHub and navigate to the **starter**.
2. Click the **Use this template** button and then select **Create a new repository**.
3. Name the new repository `<username>.github.io`, replacing `username` with your lowercase GitHub username.

### Option 2. Forking the Theme

This approach is convenient for modifying features or UI design, but presents challenges during upgrades.

1. Sign in to GitHub.
2. Fork the theme repository.
3. Name the new repository `<username>.github.io`.

## Setting up the Environment

Once your repository is created, it's time to set up your development environment.

### Using Dev Containers (Recommended for Windows)

Dev Containers offer an isolated environment using Docker, which prevents conflicts with your system.

### Setting up Natively (Recommended for Unix-like OS)

1. Follow the Jekyll installation guide to install Jekyll and ensure Git is installed.
2. Clone your repository to your local machine.
3. Run command `bundle install` in the root of your repository to install the dependencies.

## Usage

### Start the Jekyll Server

To run the site locally, use the following command:

```terminal
$ bundle exec jekyll serve
```

After a few seconds, the local server will be available at <http://127.0.0.1:4000>.

### Configuration

Update the variables in `_config.yml`{: .filepath} as needed. Some typical options include:

- `url`
- `avatar`
- `timezone`
- `lang`

### Social Contact Options

Social contact options are displayed at the bottom of the sidebar. You can enable or disable specific contacts in the `_data/contact.yml`{: .filepath} file.

## Deployment

Before deploying, check the `_config.yml`{: .filepath} file and ensure the `url` is configured correctly.

### Deploy Using GitHub Actions

1. Go to your repository on GitHub. Select the _Settings_ tab, then click _Pages_ in the left navigation bar. In the **Source** section, select **GitHub Actions** from the dropdown menu.
2. Push any commits to GitHub to trigger the _Actions_ workflow. Once the build is complete and successful, the site will be deployed automatically.

You can now visit the URL provided by GitHub to access your site.
