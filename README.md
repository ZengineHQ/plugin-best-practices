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

- [@zenginehq/frontend-config](https://www.npmjs.com/package/@zenginehq/frontend-config): for building settings forms for your plugin
- [@zenginehq/frontend-webhooks](https://www.npmjs.com/package/@zenginehq/frontend-webhooks): for managing both regular and scheduled webhooks in frontend plugins

#### Backend

- [@zenginehq/backend-firebase](https://www.npmjs.com/package/@zenginehq/backend-firebase): for retrieving settings from firebase
- [@zenginehq/backend-http](https://www.npmjs.com/package/@zenginehq/backend-http): for fetching large amounts of records from Zengine
- [@zenginehq/backend-webhooks](https://www.npmjs.com/package/@zenginehq/backend-webhooks): for managing regular and scheduled webhooks in backend services **coming soon**
