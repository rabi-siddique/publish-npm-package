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
