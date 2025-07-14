

- App Store Connect API
-  CiTagStartCondition 

Object

# CiTagStartCondition

Settings for a start condition that starts a build if a Git tag changes.

App Store Connect API 1.5+

``` source
object CiTagStartCondition
```

## Properties

`autoCancel`

`boolean`

A Boolean value that indicates whether Xcode Cloud automatically cancels or skips builds.

`filesAndFoldersRule`

CiFilesAndFoldersRule

Settings Xcode Cloud uses to determine whether a change to a tag should start a new build or not.

`source`

CiTagPatterns

The source branch name and custom patterns you configure for a workflow that starts a new build for changes to a Git tag.

## Topics

### Objects

object CiTagPatterns

Case-sensitive patterns Xcode Cloud uses to determine if a change meets tag names you configure for a workflow’s start condition.

## See Also

### Objects

object CiBranchStartCondition

Settings for a start condition that starts a build if a branch changes.

object CiPullRequestStartCondition

Settings for a start condition that starts a build if a pull request changes.

object CiScheduledStartCondition

Settings for a start condition that starts a build based on a schedule.

object CiFilesAndFoldersRule

Settings Xcode Cloud uses to determine whether a change should start a new build or not.

