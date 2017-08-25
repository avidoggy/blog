---
layout: post
title: "Using CircleCI to deploy Chalk and be hosted on Github Pages"
description: "This post will describe and step-by-step how to use CircleCI to deploy Chalk, which is a great blog template for Jekyll, and be hosted on Github Pages."
thumb_image: "documentation/sample-image.jpg"
tags: [web, chalk, circleci, githubpages]
---

Any mistakes in grammar or words spelling, please point out by pull request.

---------
<br/>

## Before starting

- *[CircleCI](https://circleci.com/)* provides a continuous integration and delivery platform to help software teams rapidly release code with confidence by automating the build, test, and deploy process.

- *[Chalk](https://github.com/nielsenramon/chalk)* is a high quality, completely customizable, performant and 100% free blog template for Jekyll.

- *[Github Pages](https://pages.github.com/)* is designed to host your personal, organization, or project pages directly from a GitHub repository.

<br/>

## Clone Chalk to local

1. I suppose you had a Github account already. If not, please [SignUp](https://github.com/join?source=header-home)

2. Fork from [nielsenramon/chalk](https://github.com/nielsenramon/chalk) and Clone

    `git clone https://github.com/<your-account>/chalk.git my-blog`

3. Following [Chalk Installation](https://github.com/nielsenramon/chalk#installation)

    ```bash
    # Install Ruby and npm
    brew install ruby
    brew install npm
    
    # Setup your environment
    cd my-blog
    bin/setup
    ```
    
    <p/>

    If you meets `limxml2` error, try `xcode-select --install`

4. Configuring your blog

    - Editing your blog's name by `name` in `_config.yml`
    - Adding GA Tracking-code by `ga_analytics` in `config.yml`
    - Using your domain by adding your domain-name in `CNAME`

5. Posting paper

    Adding markdown file in `_posts/` and following this format `<yyyy>-<MM>-<dd>-<title>.md`.

    For example:

    ```bash
    touch _posts/2017-04-01-my-first-posting.md
    ```

    <p/>

6. Adding tag

    Adding markdown file in `_my_tags/`.

    For example:

    ```bash
    echo "---
    slug: aws
    name: Amazon Web Service
    ---" > _my_tags/aws.md
    ```

    <p/>

7. Adding CirclCI

    For Automated deployment with Circle CI, please following [[Original Guide]](https://github.com/nielsenramon/kickster#automated-deployment-with-circle-ci)

## Conclusion

Chalk is realy a GREAT Github-Page template for blog.