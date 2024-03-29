A [Datasette](https://datasette.io/) instance that allows users to explore public and private files hosted by [biglocalnews.org](https://biglocalnews.org)

* Production: [datasette.biglocalnews.org](https://datasette.biglocalnews.org)
* Development: [dev-datasette.biglocalnews.org](https://dev-datasette.biglocalnews.org)
* Plugin: [simonw/datasette-big-local](https://github.com/simonw/datasette-big-local)

## Deployment

Install the dependencies.

```bash
pipenv install
```

Login to Fly.io. Our credentials are available in our password manager. Click [here](https://fly.io/docs/hands-on/install-flyctl/) for instructions on installing flyctl, the command line client for Fly.io.

```bash
flyctl auth login
```

Deploy to fly.io

```bash
# For production
pipenv run make deploy_prod
# For the dev site
pipenv run make deploy_dev
```
