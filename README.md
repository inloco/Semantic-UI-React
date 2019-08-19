# In Loco fork of [Semantic UI React](https://github.com/Semantic-Org/Semantic-UI-React)

The only purpose of this project is to change the original prefix `.ui` to our prefix `.orion`.

This project is only used by [@inloco/orion](https://github.com/inloco/orion) and should not be used standalone.

Project resources:

- npm - [@inloco/semantic-ui-react](https://www.npmjs.com/package/@inloco/semantic-ui-react)

- github - [inloco/semantic-ui-react](https://github.com/inloco/Semantic-UI-React/)

## Upgrade to a new version

When Semantic UI React releases a new version, you should follow theses steps:

1. Create a new branch from a tag: ex: `git checkout -b orion/v0.87.3 v0.87.3

2. Replace all referecences in the source code from `ui` to `orion`. Ex: [Commit](https://github.com/inloco/Semantic-UI-React/commit/d57e411440995d11ffdf5fc9671c7f12bfecf1b8)

3. Replace the package name from `semantic-ui-react` to `@inloco/semantic-ui-react`.

4. Commit and push them.

5. publish it: `yarn publish`. Use the same version of the semantic-ui-react package.

6. It is done. You can upgrade Orion package with the new version.

OBS: We do NOT create PR or merge this branch to master, since we are only replicating the versions created by Semantic UI React.
