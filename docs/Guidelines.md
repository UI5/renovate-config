# Development Conventions and Guidelines

## Linting Guidelines

Please ensure prettifing the `default.json` using [Prettier](https://prettier.io/) by execute `npm run prettier` before you commit your change.  

## Git Guidelines

### No Merge Commits

Please use [rebase instead of merge](https://www.atlassian.com/git/tutorials/merging-vs-rebasing) to update a branch to the latest main. This helps keeping a clean commit history in the project.

### Commit Message Style

This project uses the [Conventional Commits specification](https://www.conventionalcommits.org/) to ensure a consistent way of dealing with commit messages.

````
feat(default.json): Detect deprecated UI5 versions

Check the deprecation status of UI5 releases.
````

#### Structure

````
type(scope): Description
````

- required: every commit message has to start with a lowercase `type`. The project has defined a set of [valid types](../commitlint.config.mjs#L10).
- optional: the `scope` is typically the affected module. If multiple modules are affected by the commit, skip it or define a meaningful abstract scope.
- required: the `description` has to follow the Sentence Case style. Only the first word and proper nouns are written in uppercase.
