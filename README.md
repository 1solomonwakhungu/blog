# New Blog

![screenshot](https://user-images.githubusercontent.com/1177460/61880744-5b138980-aeed-11e9-9d8e-07c0b3c03cc5.png)

# Installing

```bash
# From Source
git clone <repo>
cd eleventy-starter-ghost
```

Then install dependencies

```bash
yarn
```

# Running

Start the development server

```bash
yarn start
```

You now have a completely static site pulling content from Ghost running as a headless CMS.

By default, the starter will populate content from a default Ghost install located at https://eleventy.ghost.io.

To use your own install, edit the `.env` config file with your credentials. You can find your `contentApiKey` in the "Integrations" screen in Ghost Admin. The minimum required version for Ghost is `2.10.0` in order to use this starter without issues.

# Deploy

The starter contains three config files specifically for deploying with Netlify. A `netlify.toml` file for build settings, a `headers.njk` file with default security headers set for all routes (builds to `/_headers` path), and `redirects.njk` to set Netlify custom domain redirects (builds to `/_redirects` path).

To deploy to your Netlify account, hit the button below.

Content API Keys are generally not considered to be sensitive information, they exist so that they can be changed in the event of abuse; so most people commit it directly to their `.env` config file. If you prefer to keep this information out of your repository you can remove this config and set [Netlify ENV variables](https://www.netlify.com/docs/continuous-deployment/#build-environment-variables) for production builds instead.


# Extra options

```bash
# Build the site locally
yarn build
```
