# GitHunt React

An example of a client-side app built with React 16 and Apollo Client 2.0.

See the application running live at [http://www.githunt.com](http://www.githunt.com).

[![Get on Slack](https://img.shields.io/badge/slack-join-orange.svg)](http://www.apollostack.com/#slack)
[![Build Status](https://travis-ci.org/apollostack/GitHunt-React.svg?branch=master)](https://travis-ci.org/apollostack/GitHunt-React)

Please submit a pull request if you see anything that can be improved!

## Running the app

### 1. Clone and run the GitHunt API

This repository is only the React frontend. Run the [GitHunt API](https://github.com/apollostack/GitHunt-API) first. (This is temporary, until we have a permanently hosted demo server.)

### 2. Install Node/npm

Make sure you have Node.js installed (the app has been tested with Node `8`)

### 3. Clone and install dependencies

```
git clone https://github.com/apollostack/GitHunt-React.git
cd GitHunt-React
npm install
```

### 4. Run the app

```
npm run dev
```

- Open the client at http://localhost:3000
- Click "Log in with GitHub" in the upper right corner
- You'll be presented with the seed items in the app

![GitHunt App](screenshots/GitHunt-app.png)

**Note:** If you would like to run the app using a local hostname other than `localhost`, store the new hostname in a `GITHUNT_LOCALHOST` environment variable (e.g. `export GITHUNT_LOCALHOST="local.dev"`), before starting the app.

### Hybrid Transport
GitHunt has support for hybrid transport (HTTP for queries and mutations, WebSockets for subscriptions). You can view the implementation in `src/links.js`.

#### Submit a Repo
Click the green Submit button and add repo with the username/repo-name pattern.

![GitHunt App](screenshots/GitHunt-add.png)

#### New Item
Review the new item, up vote it and visit the repo via the link.
![GitHunt App](screenshots/GitHunt-new.png)
