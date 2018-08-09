# Plugin Best Practices

> Documentation on available tools and best practices for developing Zengine Plugins.

## Generator

Whenever starting a plugin from scratch consider using the provided Yeoman [generator](https://github.com/Wizehive/generator-zn-plugin): 

```shell
npm i -g generator-zn-plugin
```

## Helper modules

There are a number of modules available on NPM in the [@zenginehq](https://www.npmjs.com/org/zenginehq) organization:

#### Frontend

- [config](https://www.npmjs.com/package/@zenginehq/frontend-config): for building settings forms for your plugin and storing them in Firebase
- [webhooks](https://www.npmjs.com/package/@zenginehq/frontend-webhooks): for managing both regular and scheduled webhooks in frontend plugins
- [bulk](https://www.npmjs.com/package/@zenginehq/frontend-bulk): for working with bulk Zengine API requests and avoiding API rate limits

#### Backend

- [firebase](https://www.npmjs.com/package/@zenginehq/backend-firebase): for reading and writing data to Firebase
- [http](https://www.npmjs.com/package/@zenginehq/backend-http): for working with the Zengine API, includes batched fetching a large amount of records
- [webhooks](https://www.npmjs.com/package/@zenginehq/backend-webhooks): for managing regular and scheduled webhooks in backend services

## Plugin Development Golden Standard

All official helper plugins created and maintained by WizeHive should adhere to the following standards (see existing backend plugins for reference):

- `README.md` file containing badges, brief information, a screenshot if applicable, examples if applicable and a link to the generated API docs
- `package.json` script to lint code using standard configs (@todo provide gist)
- Code commited using the [expected conventions](https://gist.github.com/alexweber/502494e55ebca1df855cad1e65715817) and versions maintained using `standard-version`
- `.nvm` file specifying node version to use (currently 8.x)
- 100% test coverage for backend services, using Istanbul with Coveralls
- Automatically generated API docs, hosted in Github pages
