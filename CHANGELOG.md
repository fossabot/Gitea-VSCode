# Change Log

All notable changes to the "gitea-vscode" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [0.0.2] - 2019-04-10
### Added:
- Configfile with token and repo properties
- Refresh button (Await HTTP Request)
- Multiple Pages
### Removed:
- Interval for updating

## [0.0.3] - 2019-04-10
### Added:
- Implemented [Create issue icon](./resources/dark/create.svg)
- Interval for updating (Issuelist now gets updated every ten minutes)
- Closed Issues View
- SSL server support
- License
### Refactored:
- [IssueProvider](./src/issueProvider.ts) splitted up in two parts: OpenIssuesProvider and ClosedIssuesProvider
- class Issue is now in [issue.ts](./src/issue.ts)
- organizing imports
- renaming

## [0.0.4] - 2019-04-11
### Fixed:
- [Issue 1][#1] - `\n` is now represented as ´<br/>´-tag
- [Issue 2][#2] - Markdown is now represented as HTML

## [0.0.5] - 2019-04-12
### Added:
- Child items to root items. Collapsable item now shows assignee, state, id and list all labels from the issue
- Label dependent icons
### Refactored:
- Created two methods that are used in both classes (the closed and the open issues provider)

## [0.0.6] - 2019-04-12
### Added:
- Label dependent icons now allow the user to use the colors from the Gitea server

## [0.0.7] - 2019-06-14
### Added:
- Every issue can now be opened just once at a time
### Refactored:
- Removed "filename" from `issue.ts` `labelDependentIcon()`


## [Unreleased]

- Initial release

### [0.0.6] / [0.0.7]
- From" Property of issue now displays the creater of an issue



[#1](https://github.com/IJustDev/Gitea-VSCode/issues/1)
[#2](https://github.com/IJustDev/Gitea-VSCode/issues/2)