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
- **chore**: Grunt tasks or maintenance changes that are not considered part of the codebase (editorconfig, prettier, version bumps, non-CI related files, etc).
- **ci**: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs).
- **docs**: Documentation only changes (README or Changelog).
- **feat**: A new feature.
- **fix**: A bug fix.
- **image**: Add or change image file(s).
- **perf**: A code change that improves performance.
- **refactor**: A code change that neither fixes a bug nor adds a feature.
- **remove**: The removal of a file or a feature (after a being deprecated first).
- **revert**: Revert code that was previously committed (must reference the commit ID(s) to link them).
- **security**: Improves security or resolves a security issue.
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc); or changes to CSS rules.
- **test**: Adding missing tests or correcting existing tests.

# OOP Principles

## Encapsulation

- The hiding of information from outside of the object.
  - `private` properties can only be accessed by that object.
  - `protected` properties can only be accessed by that object and any child objects that extend it.
- `public` is the default, therefore making encapsulation a conscious choice.
  - `public` properties can be accessed by any and all objects. `public` properties should be used sparingly and only in certain scenarios.
- By encapsulating the properties, it promotes the intention of creating getter and setter methods, in which there is a single point in the code where a property can be accessed and modified respectively.

## Abstraction

- Helps focus on the essential elements of an object, and hide less important details or mechanisms.
- Organises code more efficiently and extracts (*abstracts*) parts of the code into their own functions, methods, etc., using the DOT prinicple.
  - Allows a program to not worry about the details of *how* an action is performed, but only *what* action is performed.
  - A form of separation of concerns.
- Helps to construct more understandable code and promotes reusability.

## Inheritance

- Allows an object (child) to extend another object (parent).
  - The child *inherits* all the properties and methods from the parent.
  - Allows usage of the code from the parent.
  - Enables the child to override methods and properties of the parent with it's own implementation.
- Promotes reusability and avoids duplication, meaning DRYer code.

## Polymorphism

- Extends inheritance, by allowing the parent object to become an `abstract` template object.
  - Defines common methods for the child objects to *inherit* and use.
  - Defines specific `abstract` methods that the child objects *must* implement.
    - Allows child objects of different types to perform the same method but with differing implementations.
- Promotes reusability and flexibility.

## Single Responsibility

- Extends on the DOT principle.
  - A *single* file should define a *single* object.
  - An object should have only a *single* responsibility - Do One Thing.
  - An object should have a *single* reason to change.
- Promotes organisation.

