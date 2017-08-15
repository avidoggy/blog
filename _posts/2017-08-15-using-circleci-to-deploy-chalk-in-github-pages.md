---
layout: post
title: "Using CircleCI to deploy Chalk and be hosted on Github Pages"
description: "This post will describe and step-by-step how to use CircleCI to deploy Chalk, which is a great blog template for Jekyll, and be hosted on Github Pages."
thumb_image: "documentation/sample-image.jpg"
tags: [Web, Chalk, CircleCI, GitHubPages]
---

> If I have any mistakes in grammar or words spelling, please point out or pull request.

---------

## Before starting

- *[CircleCI](https://circleci.com/)* provides a continuous integration and delivery platform to help software teams rapidly release code with confidence by automating the build, test, and deploy process.

- *[Chalk](https://github.com/nielsenramon/chalk)* is a high quality, completely customizable, performant and 100% free blog template for Jekyll.

- *[Github Pages](https://pages.github.com/)* is designed to host your personal, organization, or project pages directly from a GitHub repository.

----------

## Clone Chalk to local

0. I suppose you had a Github account already. If not, please [SignUp](https://github.com/join?source=header-home)

1. Clone https://github.com/nielsenramon/chalk

    ```
    git clone https://github.com/nielsenramon/chalk.git my-blog
    ```

2. Following [Chalk Installation](https://github.com/nielsenramon/chalk#installation)

    ```
    # Install Ruby and npm
    brew install ruby
    brew install npm
    
    # Go into my-blog and setup your environment
    cd my-blog
    bin/setup
    ```
