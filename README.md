# Google Apps Script Development

![Google Apps Script Development with ES6](https://digitalinspiration.com/images/google-apps-script-development.png)

## Getting Started

1\. Clone the repository and install npm dependencies

```
git clone https://github.com/BenjjinF/apps-script-starter.git my-project
cd my-project
npm install
```

2\. Log in to Google clasp and authorize with your Google account.

```
npx clasp login
```

3\. Create a new Google Script bound to a Google Sheet (or set the type as standalone to create a standalone script in your Google Drive)

```
npm run create
```

4\. Include the necessary [OAuth Scopes](https://github.com/labnol/apps-script-starter/blob/master/scopes.md) in the [appsscript.json](https://github.com/labnol/apps-script-starter/blob/master/appsscript.json) file

5\. Push the project (development mode)

```
npm run push
```

6\. Deploy the project (production mode)

```
npm run deploy
```

#### Development vs Production mode

In the production mode, the function names and variable names are shrinked and the output code is auto-minifed. The production mode is not recommended for testing and debugging the Apps Script code.

### The .claspignore file

The `.claspignore` file allows you to specify file and directories that you do not wish to not upload to your Google Apps Script project via `clasp push`.

The default `.claspignore` file of the Apps Script Starter kit will push all the JS and HTML inside the `rootDir` folder and ignore all the other files.

## Credits

Adapted from Amit Agarwal's [app-script-starter](https://github.com/labnol/apps-script-starter)