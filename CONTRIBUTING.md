# Contributing

1. Create a fork of this project. [Github Documentation](https://docs.github.com/en/pull-requests/how-tos/work-with-forks/fork-a-repo)
1. Create a new feature branch. [Git Flow Documentation](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)
1. Start modifying the stylesheets in `styles/websites` and also update `data/ContentScripts.json` as needed.
1. Commit & push your changes to your fork.
1. Create a Pull request from your feature branch.

## Guidelines

- Use `var(--transparent-background)`/`var(--text-color)` where possible in your stylesheets. Fall back to `@media-query prefers-scheme dark` when the plugin colors don't suffice.

## Testing your modifications

> [!TIP]
> Make sure to disable dynamic transparency when testing.

### Utilizing temporary install

Make sure to run the following commands:
```bash
npm install
npm run build
```

- open Firefox
- enter `about:debugging` in the URL bar
- click "This Firefox"
- click "Load Temporary Add-on"
- open the extension's directory and select any file inside the extension,or select the packaged extension (.zip file).
- head to one of the sites you modified (if they were already open, make sure to refresh)

[Firefox Documentation](https://extensionworkshop.com/documentation/develop/temporary-installation-in-firefox/)

### Setting up web-ext
https://extensionworkshop.com/documentation/develop/getting-started-with-web-ext/

## Before submitting

- Have you checked it looks good with both color-schemes (dark/light). (browser dev-tools usually allow you to spoof that)
- 
