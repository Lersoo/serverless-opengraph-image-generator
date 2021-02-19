# Serverless OpenGraph Image Generator

### Usage

1. `index.html` is the default template for generating images. Open and edit it as you like. You can also create your own.

2. Run:
```sh
yarn predeploy # Will clone latest chromium and zip it for AWS Lambda Layer
sls deploy # Deploy Serverless stack and push Lambda layer with Puppeteer

curl <DEPLOYED_ENDPOINT>?title=This is awesome!
```

By default, Puppeteer will render `index.html` file but you can also use `template` parameter to open another HTML file, like so:

```
https://<your_endpoint>?template=twiddb.html?title=ANOTHER%20TEMPLATE
```

### Author

This repo has been forked from 👤 [**Dynobase**](https://dynobase.dev)
