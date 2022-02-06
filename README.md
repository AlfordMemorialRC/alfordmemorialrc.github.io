---
title: README
layout: plain-noindex
---

# totr-radio
Here is the Alford Memorial Radio Club website in HTML/Markdown!

## Setup For Local Development

### 1. Install Prerequisites
* Install [Docker](https://docs.docker.com/engine/installation/) for your Operating System.   
> **Windows and Mac users should install Docker Desktop!**   
> **Linux users should install from the distribution repositories!**  
* (Linux) Install [Docker Compose](https://docs.docker.com/compose/install/)    
> **Only Linux host systems require a separate installation of docker-compose!**   
> **Docker Desktop includes a bundled *Docker Compose*!**   

### 2. Establish Local Repository
1. On GitHub, fork <a href="https://github.com/AlfordMemorialRC/totr-radio" title="totr-radio" target="_blank" rel="noopener">this repo</a>.

1. Clone the fork to your local machine.

1. In Terminal, navigate to the repo directory on your local machine.

### 3. Configuration Step by Step
1. Generate a [new GitHub Token](https://github.com/settings/tokens/new).

1. Add your secrets to your `.env` file. If `.env` does not yet exist in your project directory, the below command will create it automatically. Lets add the required secret, `JEKYLL_GITHUB_TOKEN`:

   ```bash
   echo 'JEKYLL_GITHUB_TOKEN=[REPLACE_WITH_TOKEN]' >> .env
   ```

   Using `0jcdahcl66mvmyahj68xngnug0db19y2xvdm1zlb` as an example:

   ```bash
   echo 'JEKYLL_GITHUB_TOKEN=0jcdahcl66mvmyahj68xngnug0db19y2xvdm1zlb' >> .env
   ```   

### 4. Build and serve the site locally from [http://localhost:4000](http://localhost:4000)
```
$ docker-compose up -d
```   
**Then, navigate to** <a href="http://localhost:4000/" title="Jekyll" rel="noopener" target="_blank"><b>http://localhost:4000</b></a> **with a browser.**   
> As you make updates, the changed pages will be automatically regenerated.

## Changes To Site Configuration (*changes to _config.yml*):
> It may take up to 20-30 seconds to complete.   

```
$ docker-compose restart
```

## View site-generator log for troubleshooting:
```
$ docker-compose logs -f
```

---
