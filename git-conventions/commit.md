## Format of the commit message:

```bash
<type>(<scope>): <subject>
```

> Consider each commit should do just **one** task.

#### Allowed `<type>` values:

* **feat** for a new feature for the user, not a new feature for build script. Such commit will trigger a release bumping a MINOR version.
* **fix** for a bug fix for the user, not a fix to a build script. Such commit will trigger a release bumping a PATCH version.
* **perf** for performance improvements. Such commit will trigger a release bumping a PATCH version.
* **docs** for changes to the documentation.
* **lint** for formatting changes, missing semicolons, etc.
* **refactor** for refactoring production code, e.g. renaming a variable.
* **test** for adding missing tests, refactoring tests; no production code change.

#### Allowed `<scope>` values:

* **infra**  infrastructure
* **layout**  layout
* **comp**  component
* **imp**  implementation
* **mix** mixture:  mixture of two or more than above scopes


> The subject cannot be longer than 72 characters. It must be in simple present tens always (e.g. fixes, adds and so on).

>  type and scope should always be lowercase as shown in the example below.

> The `<scope>` can be empty, in which case the parentheses are omitted.

> Don't use **mix** scope until it really be necessary.

## Example commit message:

```
fix(infra): configs eslint
```

This document is based on [Angular Commit Message Format]. See the [commit history] for examples of properly-formatted commit messages.

[Angular Commit Message Format]: https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit
[commit history]: https://github.com/karma-runner/karma/commits/master
