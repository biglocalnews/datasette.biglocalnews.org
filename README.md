# datasette.biglocalnews.org

A [Datasette](https://datasette.io/) instance that allows users to explore public and private files hosted by [biglocalnews.org](https://biglocalnews.org)

## Deployment

Install the dependencies.

```bash
pipenv install
```

Login to Fly.io. Our credentials are available in our password manager.

```bash
flyctl auth login
```

Deploy to fly.io

```bash
pipenv run make deploy
```
