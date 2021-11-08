## Branch type categories

 1. ***Code flow types***: These branches which we expect to be permanently available on the repository follow the flow of code changes starting from development until the production.

 2. ***Temporary types***: As the name implies, these are disposable branches that can be created or deleted when needed.

### Code flow types:

 - **development**: All new features and bug fixes should be brought to this branch.

 - **test**: Contains all codes ready for QA testing.

 - **staging** (optional): It contains tested features that the stakeholders wanted to be available either for a demo or a proposal before elevating into the production. Decisions are made here if a feature should be finally brought to the production code.
 
 - **master**: The production branch, if the repository is published, this is the default branch being presented.

> Except for Hotfixes, we want our codes to follow a one-way merge starting from development > test > staging > master.

### Temporary types:

 - **feature**: Any code changes for a new module or use case should be done on a feature branch. This branch is created based on the current `development` branch. When all changes are 'Done', a PR is needed to put all of these to the development branch.
 
 - **bugfix**: If the code changes made from the `feature` branch were rejected after a release, sprint or demo, any necessary fixes after that should be done on this branch.
 
 - **hotfix**: If there is a need to fix a blocker, do a temporary patch, apply a critical framework or configuration change that should be handled immediately, it should be created as a *hotfix*. It does not follow the scheduled integration of code and could be merged directly to the `master` branch, then on the `development` branch later.
 
 - **experimental**: Any new feature or idea that is not part of a release or a sprint. A branch for playing around.
 
 - **release**: A branch for tagging a specific release version.
 
 - **merging**: A temporary branch for resolving merge conflicts, usually between the latest development and a feature or Hotfix branch. This can also be used if two branches of a feature being worked on by multiple developers need to be merged, verified and finalized.


## Format of the branch name:

```bash
<author-name>-<type>-<subject>-<ID>
```

> The `<ID>` can be empty (e.g. if the change isn't assign to a JIRA task ).

> The `<subject>` must be short and rational.

## Examples:

```
alireza-feature-toast-23
taher-merge-device-support-35
alireza-bugfix-more-gray-shades
taher-hotfix-scaling-threshold
```

This document is based on [Git Branch Naming Convention](https://dev.to/couchcamote/git-branching-name-convention-cch).
