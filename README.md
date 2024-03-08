# Wei README

> This works with Okta Code Flow (no PKCE) client application
> Okta interface only allows code flow if it's clinet / server app
> make sure to use that to create the app
> after that, run the app, after login, you should see the auth code returned

Install okta cli tool

`brew install --cask oktadeveloper/tap/okta`

- Login to okta dev account, 
    - create okta cli api key

- use Okta cli 
    - `okta login` (use okta domain and cli api key)
    - `okta start express` (cli creates a express folder)

- cd to `express` folder

- `npm install`
- `npm start run`
- access localhost port 3000

			

# Node.js Express Quickstart Sample Code for Integrating with Okta using the Redirect Model

This repository contains a sample of integrating with [Okta](https://www.okta.com/) for authentication using [the redirect model in a Node.js Express app](https://developer.okta.com/docs/guides/sign-into-web-app-redirect/node-express/main/).

Read more about getting started with Okta and authentication best practices on the [Okta Developer Portal](https://developer.okta.com).

This code sample demonstrates
* Configuring Okta
* Sign-in and sign-out
* Protecting routes
* Displaying user profile information from the ID Token

## Prerequisites

Before running this sample, you will need the following:

* [The Okta CLI Tool](https://github.com/okta/okta-cli#installation)
* An Okta Developer Account (create one using `okta register`, or configure an existing one with `okta login`)

## Get the Code

Grab and configure this project using `okta start express`.

Follow the instructions printed to the console.

## Run the Example

To run this application, install its dependencies:

```
npm install
```

With variables set, start your app:

```
npm start
```

Navigate to http://localhost:3000 in your browser.

If you see a home page that prompts you to login, then things are working!  Clicking the **Log in** button will redirect you to the Okta hosted sign-in page.

You can sign in with the same account that you created when signing up for your Developer Org, or you can use a known username and password from your Okta Directory.

> **Note:** If you are currently using your Developer Console, you already have a Single Sign-On (SSO) session for your Org.  You will be automatically logged into your application as the same user that is using the Developer Console.  You may want to use an incognito tab to test the flow from a blank slate.

## Helpful resources

* [Learn about Authentication, OAuth 2.0, and OpenID Connect](https://developer.okta.com/docs/concepts/)
* [Get started with Express](https://expressjs.com/en/starter/installing.html)

## Help

Please visit our [Okta Developer Forums](https://devforum.okta.com/).
