
## Welcome to My Blog
Hello and welcome to my blog! My name is Ogochukwu Ozotta, and I am a DevOps/Site Reliability Engineer with a passion for Cloud, DevOps, Data Engineering, and Machine Learning. This blog is where I share insights, tutorials, and discussions on topics that I am passionate about, including:
- **Cloud Infrastructure:** Best practices and strategies for AWS, Azure, and GCP.
- **DevOps Automation:** Streamlining CI/CD pipelines, infrastructure as code (Terraform, Ansible), and container orchestration with Kubernetes.
- **Data Science & MLOps:** Exploring data engineering pipelines, cloud-based AI solutions, and the convergence of DevOps and DataOps.
- **Site Reliability Engineering (SRE):** Insights on system reliability, cloud-native applications, and real-world experiences managing scalable infrastructure.

## Blog Post
- [Machine Learning & AI Services: Exploring Alternatives and Differences Between AWS and Azure](_posts/2024-09-30-Machine-Learning-AI-Services.md)


## Blog Highlights
### DevOps, Cloud, and Automation
I leverage years of hands-on experience to bring you content on the latest trends and techniques in cloud automation, container orchestration, and DevOps practices. Expect blog posts on:
- **CI/CD Pipelines:** Automating deployments using Jenkins, GitHub Actions, and Azure DevOps.
- **Containerization:** Best practices for Docker, Kubernetes, Helm charts, and Istio service mesh.
- **Infrastructure as Code:** Step-by-step guides on using Terraform and Ansible for cloud provisioning and management.

### Data Science & MLOps
With a growing focus on **MLOps**, I dive into topics at the intersection of data science and operations, including:
- Automating data workflows with AWS Lambda, Glue, and Kubernetes.
- Building scalable, reliable machine learning pipelines in the cloud.
- Integrating data engineering best practices to improve system performance and scalability.

## About Me
I have a PhD in Petroleum Engineering and a diverse background in Cloud Computing and Infrastructure Engineering. My professional experience spans various industries, including academia, fintech, energy, software development, and cloud infrastructure for large-scale enterprises. In my current role as a **Site Reliability Engineer**, I focus on ensuring the availability and reliability of cloud-native applications using cutting-edge DevOps tools and methodologies.
### Professional Journey
- **Site Reliability Engineer**  
 Led Kubernetes deployments and maintaining scalable, reliable cloud infrastructures.
- **Senior DevOps/Cloud Engineer**  
 Developed microservices architecture and led cloud migrations using EKS and Istio.
- **Infrastructure Engineer**   
 Orchestrated cloud automation with AWS and Kubernetes, streamlining real-time data streaming.

## Stay Connected
If you’re interested in staying updated with my latest blog posts, feel free to **follow me on GitHub** or reach out to me directly through **ogochukwu.ozotta@gmail.com**. I’m always open to collaborations, feedback, and discussions on the evolving landscape of DevOps, Cloud, and Data Science.


_Thanks for visiting my blog! Let’s build something amazing together._



# Academic Pages
**Academic Pages is a Github Pages template for academic websites.**

# Getting Started

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Click the "Use this template" button in the top right.
1. On the "New repository" page, enter your repository name as "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and add your content.
1. Upload any files (like PDFs, .zip files, etc.) to the `files/` directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.
1. Check status by going to the repository settings, in the "GitHub pages" section
1. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## Running locally

When you are initially working your website, it is very useful to be able to preview the changes locally before pushing them to GitHub. To work locally you will need to:

1. Clone the repository and made updates as detailed above.
1. Make sure you have ruby-dev, bundler, and nodejs installed
    
    On most Linux distribution and [Windows Subsystem Linux](https://learn.microsoft.com/en-us/windows/wsl/about) the command is:
    ```bash
    sudo apt install ruby-dev ruby-bundler nodejs
    ```
    On MacOS the commands are:
    ```bash
    brew install ruby
    brew install node
    gem install bundler
    ```
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `jekyll serve -l -H localhost` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.

If you are running on Linux it may be necessary to install some additional dependencies prior to being able to run locally: `sudo apt install build-essential gcc make`

## Using Docker

Working from a different OS, or just want to avoid installing dependencies? You can use the provided `Dockerfile` to build a container that will run the site for you if you have [Docker](https://www.docker.com/) installed.

Start by build the container:

```bash
docker build -t jekyll-site .
```

Next, run the container:
```bash
docker run -p 4000:4000 --rm -v $(pwd):/usr/src/app jekyll-site
```

# Maintenance

Bug reports and feature requests to the template should be [submitted via GitHub](https://github.com/academicpages/academicpages.github.io/issues/new/choose). For questions concerning how to style the template, please feel free to start a [new discussion on GitHub](https://github.com/academicpages/academicpages.github.io/discussions).

This repository was forked (then detached) by [Stuart Geiger](https://github.com/staeiou) from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License (see LICENSE.md). It is currently being maintained by [Robert Zupko](https://github.com/rjzupkoii) and additional maintainers would be welcomed.

## Bugfixes and enhancements

If you have bugfixes and enhancements that you would like to submit as a pull request, you will need to [fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) this repository as opposed to using it as a template. This will also allow you to [synchronize your copy](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) of template to your fork as well.

Unfortunately, one logistical issue with a template theme like Academic Pages that makes it a little tricky to get bug fixes and updates to the core theme. If you use this template and customize it, you will probably get merge conflicts if you attempt to synchronize. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch.

---
<div align="center">
    
![pages-build-deployment](https://github.com/academicpages/academicpages.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)
[![GitHub contributors](https://img.shields.io/github/contributors/academicpages/academicpages.github.io.svg)](https://github.com/academicpages/academicpages.github.io/graphs/contributors)
[![GitHub release](https://img.shields.io/github/v/release/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io/releases/latest)
[![GitHub license](https://img.shields.io/github/license/academicpages/academicpages.github.io?color=blue)](https://github.com/academicpages/academicpages.github.io/blob/master/LICENSE)

[![GitHub stars](https://img.shields.io/github/stars/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io)
[![GitHub forks](https://img.shields.io/github/forks/academicpages/academicpages.github.io)](https://github.com/academicpages/academicpages.github.io/fork)
</div>
