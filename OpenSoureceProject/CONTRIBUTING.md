# Contributing to Our Project

We would love for you to contribute to Our Project and help make it even better than it is today! As a contributor, here are the guidelines we would like you to follow:

- Code of Conduct
- Question or Problem?
- Issues and Bugs
- Feature Requests
- Coding Rules
- Commit Message Guidelines

## Code of Conduct

## Got a Question or Problem?

## Found a Bug?

## Missing a Feature?

## Submission Guidelines

### Submitting an Issue

### Submitting a Pull Request (PR)

## Coding Rules

## Commit Message Guidelines

We have very precise Rules over how our git commit messages can be formatted. This leads to more readable messages that are easy to follow when looking through the project history. But also, we use the git commit messages to generate the Angular change log.

### Commit Message Format

Each commit message consistes of a header, a body and a footer. The header has a special fformat that includes a type, a scope and a subject:

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

The header is mandatory and the scope of the header is optional.

Any line of the commit message cannot be longer 100 characters! This allows the message to be easier to read on Github as well as in various git tols.

Footer should contain a [closing refreence to an issue]() is any.

Samples:(even more [samples]())

```
docs(changelog): update change log to beta.5
```

```
fix(release): need to depend on latest rxjs and zone.js

The version in our package.json gets copied to the one we publish, and users need the latest of these.
```

### Revert

If the commit reverts a previous commit, it should begin with `revert:`, followed by the header of the reverted commit. In the body it should say: `This reverts commit <hash>.`, where the hash is the SHA of the commit being reverted.

### Type

Must be one of the following:

- build: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
- ci: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
- docs: Documentation only changes
- feat: A new feature
- fix: A bug fix
- perf: A code change that improves performance
- refactor: A code change that neither fixes a bug nor adds a feature
- style: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- test: Adding missing tests or correcting existing tests

### Scope

The scope should be the name of the npm package affected (as perceived by person reading changelog generated from commit messages).

The following is the list of supported scopes:

- animations
- common
- compiler
- compiler-cli
- core
- forms
- http
- language-service
- platform-browser
- platform-browser-dynamic
- platform-server
- platform-webworker
- platform-webworker-dynamic
- router
- service-worker
- upgrade

There are currently a few exceptions to the "use package name" rule:

- packaging: used for changes that change the npm package layout in all of our packages, e.g. pulbic path changes, package.json changes done to all packages, d.ts file/format changes, changes to bundles, etc.
- changelog: used for updating the release notes in CHANGELOG.md
- aio: used for docs-app (angular.io) related changes within the /aio directory of the repo
- none/empty string: useful for `style`, `test` and `refactor` changes that are done across all packages (e.g. `style: add missing semicolons`)

### Subject

The subject contains succinct description of the change:

- use the imperative, persent tense: "change" not "changed" nor "changes"
- don't capitalize first letter
- no dot (.) at the end

### Body

Just as in the subject, use the imperative, persent tense: "change" not "changed" nor "changes". The body should include the motivation for the change and contrast this with previous behavior.

### Footer

The footer should contain any information about Breaking Changes and is also the place to reference GitHub issues that this comit Closes.

Breaking Changes should start with the word `BREAKING CHANGE:` with a space or two newlines. The rest of the commit message is then used for this.

A detailed explanation can be found in this [document]()

## Signing the CLA

Please sign our Contributor License Agreement (CLA) before sending pull requests. For any code changes to be accepted, the CLA must be signed. It's a quick process, we promise!

- For individuals we have a [simple click-through form.]()
- For corporations we'll need you to [print, sign and one of scan+email, fax or mail the form.]()
