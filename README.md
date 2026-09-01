
## Updating the GitHub Pages Custom Domain (DNS)

The site is deployed to `blog.cloudcorehub.com` via GitHub Pages with AWS Route 53 managing DNS. To change the custom domain, update all three of the following:

### 1. AWS Route 53

1. Go to **Route 53 → Hosted zones → `cloudcorehub.com`**
2. Delete or update the existing subdomain CNAME record
3. Create a new record:
   - **Name**: `blog` (or whatever subdomain you want)
   - **Type**: `CNAME`
   - **Value**: `ogochukwu-ozotta.github.io`
   - **TTL**: `300`

### 2. GitHub Pages Settings

1. Go to the repo on GitHub → **Settings → Pages**
2. Under **Custom domain**, enter the new subdomain (e.g. `blog.cloudcorehub.com`)
3. Click **Save** — GitHub will verify DNS and provision a TLS certificate automatically

### 3. Repo files

Update the domain in two files:

- **`CNAME`** (repo root): set the file contents to the new domain, e.g. `blog.cloudcorehub.com`
- **`_config.yml`** line 15: update `url` to `https://blog.cloudcorehub.com`

Commit and push both changes to `main` to complete the update.

---

## Running locally

When you are initially working your website, it is very useful to be able to preview the changes locally before pushing them to GitHub. To work locally you will need to:

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
2. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
3. Run `bundle exec jekyll serve` or `jekyll serve -l -H localhost` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.

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
# This is Commit 



