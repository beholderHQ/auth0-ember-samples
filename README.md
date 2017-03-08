# Auth0 Ember Calling an API

This sample demonstrates how to make secure calls to an API after authenticating a user with Auth0. The calls to the API are made with the user's `access_token`. 

## Getting Started

If you haven't already done so, [sign up](https://auth0.com) for your free Auth0 account and create a new client in the [dashboard](https://manage.auth0.com). Find the **domain** and **client ID** from the settings area and add the URL for your application to the **Allowed Callback URLs** box. Which will be `http://localhost:4200`.

You must ensure that the APIs section is enabled in your Auth0 dashboard. To do so, go to the [Advanced Settings](https://manage.auth0.com/#/account/advanced) area and verify that **Enable APIs Section** is switched on. Next, navigate to APIs in the sidebar and create a new API. The identifier for your API will be required later.

## Set the Client ID and Domain in the `.env` file

A `.env.example` file is provided at the root of the application. This file provides your application's credentials to the small Node server located in `index.js`.

Rename `.env.example` to `.env` with your credentials filled in.

This file has two values, `AUTH0_AUDIENCE` and `AUTH0_DOMAIN`. The value for `AUTH0_AUDIENCE` is the identifier used for an API that you create in the Auth0 dashboard.

## Run the Application

The ember development server that comes with ember addon can be used to serve the application.

```bash
npm start
```

The application will be served at `http://localhost:4200`.

## Ember Adapter

See [adapter](./adapter/application.js) for an example

## Ember Application Route

See [route](./app/routes/application.js) for an example

## Ember Data
See [route](./app/routes/protected.js) for an example

## What is Auth0?

Auth0 helps you to:

* Add authentication with [multiple authentication sources](https://docs.auth0.com/identityproviders), either social like **Google, Facebook, Microsoft Account, LinkedIn, GitHub, Twitter, Box, Salesforce, amont others**, or enterprise identity systems like **Windows Azure AD, Google Apps, Active Directory, ADFS or any SAML Identity Provider**.
* Add authentication through more traditional **[username/password databases](https://docs.auth0.com/mysql-connection-tutorial)**.
* Add support for **[linking different user accounts](https://docs.auth0.com/link-accounts)** with the same user.
* Support for generating signed [Json Web Tokens](https://docs.auth0.com/jwt) to call your APIs and **flow the user identity** securely.
* Analytics of how, when and where users are logging in.
* Pull data from other sources and add it to the user profile, through [JavaScript rules](https://docs.auth0.com/rules).

## Create a free Auth0 account

1. Go to [Auth0](https://auth0.com/signup) and click Sign Up.
2. Use Google, GitHub or Microsoft Account to login.

## Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section. Please do not report security vulnerabilities on the public GitHub issue tracker. The [Responsible Disclosure Program](https://auth0.com/whitehat) details the procedure for disclosing security issues.

## Author

[Auth0](auth0.com)

## License

This project is licensed under the MIT license. See the [LICENSE](LICENSE.txt) file for more info.
