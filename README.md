
## Plugin Database for [Millennium](https://github.com/SteamClientHomebrew/Millennium)

> [!NOTE]
> This repository solely exists for developers to submit plugins.<br>
> Download & install plugins from https://steambrew.app/plugins

&nbsp;

## Introduction

Welcome to the official [Millennium](https://github.com/SteamClientHomebrew/Millennium) Plugin Database — a centralized repository that manages and curates all community and official plugins for [Millennium](https://github.com/SteamClientHomebrew/Millennium).
This repository exists to provide a secure, version-controlled collection of plugins that are approved for use with Millennium. Each plugin is tracked as a Git submodule, allowing us to:

* Independently version plugins without relying on the latest changes from their original repositories.
* Manually review all plugin updates before they reach end users, ensuring code integrity and preventing malicious behavior.
* Provide a consistent, reliable plugin experience across all installations of Millennium.

Whether you're a plugin developer submitting updates or a user browsing available extensions, this database serves as the trusted source for all Millennium-compatible plugins.

&nbsp;

### Submitting A Plugin

To submit a plugin to Millennium's plugin repository, open a pull request that adds your plugin as a submodule using the command
`git submodule add https://github.com/YourUsername/YourRepository your-plugin`
inside the `plugins` directory.

This will attach your repository from a specific commit, meaning when you update your repository, the changes won't be reflected here, unless you open a pull request to update it.
This is in place to prevent malicious code by forcing us to audit all of your code changes.

&nbsp;

### Updating Your Plugin

Once you have your submodule added, in order to update it,
change directory to `plugins/your-plugin`, checkout the branch you wish to use and pull:
```
git checkout your-plugin-branch
git pull
```
This should update your plugin to the latest version. Commit the change and open a pull request.

&nbsp;

In case you wish to clone plugins at their attached commits, run `git submodule update --init`.
