# In Loco fork of [Semantic UI React](https://github.com/Semantic-Org/Semantic-UI-React)

The only purpose of this project is to change the original prefix `.ui` to our prefix `.orion`.

This project is only used by [@inloco/orion](https://github.com/inloco/orion) and should not be used standalone.

Project resources:

- npm - [@inloco/semantic-ui-react](https://www.npmjs.com/package/@inloco/semantic-ui-react)

- github - [inloco/semantic-ui-react](https://github.com/inloco/Semantic-UI-React/)

## Upgrade to a new version

Let's assume that your fork's remote is named **fork** and the original remote is named **semantic**. Let's also assume that the new version launched by `semantic-ui-react` is **v0.87.3**. You should follow theses steps:

1. Fetch tags from Semantic: `git fetch semantic --tags`.

2. Create a new branch from a tag: ex: `git checkout -b orion/v0.87.3 v0.87.3`.

3. Cherry-pick [this commit](https://github.com/inloco/Semantic-UI-React/commit/d3eefefb9dfc4f47429d0c9a2379c1d125c41db9) and fix any conflicts that shows up (there will probably be one on `package.json` due to the name/version changes): `git cherry-pick d3eefefb9dfc4f47429d0c9a2379c1d125c41db9`.

4. Publish it running `npm publish`.

5. It is done. You can upgrade Orion package with the new version.

OBS: We do NOT create PR or merge this branch to master, since we are only replicating the versions created by Semantic UI React.
