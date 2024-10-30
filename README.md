# Next.js + Contentlayer
A template with Next.js 13 app dir, Contentlayer, Tailwind CSS and dark mode.
https://scrawny-portugal-faint.functions.on-fleek.app/

## Prerequisites 
- Node 18+
- Fleek Account
- [Fleek CLI](https://www.npmjs.com/package/@fleek-platform/cli)
- [Fleek Next Adapter](https://www.npmjs.com/package/@fleek-platform/next)

## Getting Started
1. Fork the repository
2. Clone the repository by running the following command:
```bash
git clone https://github.com/<your-id>/fleek-contentlayer.git
```
3. Enter the correct directory, install dependencies and run locally:
```bash
cd fleek-contentlayer
pnpm i
pnpm run dev
```
3. Ensure that you install the Fleek CLI and the Fleek Next Adapter:
```bash
// local installation
npm i @fleek-platform/cli
npm i @fleek-platform/next

// global installation
npm i -g @fleek-platform/cli
npm i -g @fleek-platform/next
```
💡: you can check the Fleek CLI version by running fleek -v. Any version >= 2.10.1 should be good. As for the Fleek Next adapter, you can check the Fleek Next Adapter version by running fleek-next -v. Any version >= 1.0.6 should be good.

## Building and Deploying on Fleek

Get a PAT (Personal Access Token). Run `fleek PAT create`, give it a name, login in to the platform, and copy your PAT.

Then run `export FLEEK_TOKEN=<your personal access token>` in your terminal to set your environment variables.


Then create a project ID. Run `fleek projects create`, give it a name, and copy your ID.

Then create a `fleek.json` file. Paste this in:

```bash
{
    "FLEEK_PROJECT_ID": "<project_id>"
}
```

Then run `fleek-next deploy`
