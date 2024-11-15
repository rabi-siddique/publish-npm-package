# Publishing the package manually

# 1. Log in to npm

Before you publish, ensure that you are logged in to npm with the account that owns the `@rabi-siddique` scope:

```bash
npm login
```

Follow the prompts to enter your username, password etc.

# 2. Publish Your Package

Once you are logged in and your `package.json` is correctly set up, try publishing the package with public access:

```bash
npm publish --access public
```

This command explicitly sets the package to be public, allowing anyone to install it without facing access restrictions.

# 3. Releasing a new version

Attempting to publish the package without updating the version number in package.json will result in the following error:
![403 Forbidden](./media/403.png)

To successfully publish, increment the version number in `package.json` to a new value that differs from the previous release. This change ensures that npm recognizes it as a new version, allowing the publication to proceed without errors.

You have the flexibility to choose any version number when publishing your package. For example, if your initial release was version `1.0.1`, you could choose to update it to `10.0.5` for a subsequent release:
![Version](./media/version.png)

npm allows version downgrades. You can publish a lower version, such as `3.0.5`, even after releasing a higher version like `10.0.5`, and it will still be processed successfully.
