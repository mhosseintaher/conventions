Millions, maybe billions of lines of code are written every day, and each developer has his/her own way of writing.
Existence of a set of conventions is a *good to have* for developers community, but it's a **must to have** for each team.
These are just some conventions we set for our team.

> Each commit should do just **one** task.

## Format of the commit message:
```bash
<type>(<scope>){<ID>}: <subject>
```

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
* **WIP** work in progress:  mixture of two or more than above scopes


> The subject cannot be longer than 72 characters. It must be in simple present tens always (e.g. fixes, adds and so on).

> The `<ID>` can be empty (e.g. if the change isn't assign to a JIRA task ), in which case the curly braces are omitted. type and scope should always be lowercase as shown in the example below.

> The `<scope>` can be empty too, in which case the parentheses are omitted.

> Don't use **WIP** scope until it really be necessary.

## Example commit message:

```
fix(infra){#21}: configs eslint
```



This document is based on [Angular Commit Message Format]. See the [commit history] for examples of properly-formatted commit messages.

[Angular Commit Message Format]: https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit
[commit history]: https://github.com/karma-runner/karma/commits/master
