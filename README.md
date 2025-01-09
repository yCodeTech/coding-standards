# Coding Standards
This is a little repo to document my coding standards and styles for easy reference.


## Indentation
Tabs

1 Tab = 4 spaces

## Curly brackets
Start curly brackets on if else blocks and functions should be on the same line as the declaration with a space before the curly bracket.

```js

if () {
else {

function thing() {
```

## else
`else if` and `else` blocks should be on a new line after the previous closing curly bracket

```js
if () {
}
else if () {
}
else {
}
```


# Git Commits
I use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) with the extra commit types as [described in Angular](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#type) and also some from the [Medium article - Conventional Commits: A Better Way ](https://medium.com/neudesic-innovation/conventional-commits-a-better-way-78d6785c2e08).

## Commit types

- **build**: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm).
- **ci**: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs).
- **docs**: Documentation only changes (README or Changelog).
- **feat**: A new feature.
- **fix**: A bug fix.
- **perf**: A code change that improves performance.
- **refactor**: A code change that neither fixes a bug nor adds a feature.
- **remove**: The removal of a file or a feature (after a being deprecated first).
- **revert**: Revert code that was previously committed (must reference the commit ID(s) to link them).
- **security**: Improves security or resolves a security issue.
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc).
- **test**: Adding missing tests or correcting existing tests.
