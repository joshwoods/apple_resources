

- App Store Connect API
-  CiPullRequestStartCondition 

Object

# CiPullRequestStartCondition

Settings for a start condition that starts a build if a pull request changes.

App Store Connect API 1.5+

``` source
object CiPullRequestStartCondition
```

## Properties

`destination`

CiBranchPatterns

The destination branch name and custom patterns you configure for a workflow that starts a new build for changes to a pull request.

`filesAndFoldersRule`

CiFilesAndFoldersRule

The custom rule that determines whether Xcode Cloud starts a build or not based on a pull request’s changes to files.

`source`

CiBranchPatterns

The source branch name and custom patterns you configure for a workflow that starts a new build for changes to a pull request.

`autoCancel`

`boolean`

A Boolean value that indicates whether Xcode Cloud automatically cancels or skips builds.

## See Also

### Objects

object CiBranchStartCondition

Settings for a start condition that starts a build if a branch changes.

object CiTagStartCondition

Settings for a start condition that starts a build if a Git tag changes.

object CiScheduledStartCondition

Settings for a start condition that starts a build based on a schedule.

object CiFilesAndFoldersRule

Settings Xcode Cloud uses to determine whether a change should start a new build or not.

