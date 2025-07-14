

- App Store Connect API
-  CiBranchStartCondition 

Object

# CiBranchStartCondition

Settings for a start condition that starts a build if a branch changes.

App Store Connect API 1.5+

``` source
object CiBranchStartCondition
```

## Properties

`autoCancel`

`boolean`

A Boolean value that indicates whether Xcode Cloud automatically cancels or skips builds.

`filesAndFoldersRule`

CiFilesAndFoldersRule

Settings Xcode Cloud uses to determine whether a change to a branch should start a new build or not.

`source`

CiBranchPatterns

The source branch name and custom patterns you configure for a workflow that starts a new build for changes to a branch.

## Topics

### Objects

object CiBranchPatterns

Case-sensitive patterns Xcode Cloud uses to determine if a change meets branch names you configure for a workflow’s start condition.

## See Also

### Objects

object CiTagStartCondition

Settings for a start condition that starts a build if a Git tag changes.

object CiPullRequestStartCondition

Settings for a start condition that starts a build if a pull request changes.

object CiScheduledStartCondition

Settings for a start condition that starts a build based on a schedule.

object CiFilesAndFoldersRule

Settings Xcode Cloud uses to determine whether a change should start a new build or not.

