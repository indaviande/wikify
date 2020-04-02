# Wikify
Wikify is a 100% static Wiki "generator", built for Netlify, with modified versions of [Docsify](https://docsify.js.org), Netlify CMS, and the Netlify Identity Widget. It is a single-page wiki, and the docs are made from Markdown files.

## Getting Started
1. First off, [deploy this repository to Netlify](https://app.netlify.com/start/deploy?repository=https://github.com/TristianK3604/wikify).
2. After your site has been deployed, you need to enable the following settings:
  - Identity
  - Git Gateway
3. Create an account for yourself (or accept the invite that should have been sent to you when you enabled Identity)
4. Manage your wiki posts at https://yoursite.com/manage

## Recommendations
For a wiki where you want to have posts approved before they are published, add this line to the `manage/config.yml` file:
````
publish_mode: editorial_workflow
````
For a private wiki (only invited users can create posts), set the registration mode to **invite only** in your Identity settings.

More documentation coming soon

## Todo

- [ ] Add Netlify GoTell Comments
- [ ] Wikify Manager Redesign
- [ ] Use JS API to replace `#` with a better looking url (`mysite.com/thisdoc` rather than `mysite.com/#/thisdoc`) (Currently working on)
