

- App Store Connect API
-  CiFilesAndFoldersRule 

Object

# CiFilesAndFoldersRule

Settings Xcode Cloud uses to determine whether a change should start a new build or not.

App Store Connect API 1.5+

``` source
object CiFilesAndFoldersRule
```

## Properties

`matchers`

`[`CiStartConditionFileMatcher`]`

Directory and file information Xcode Cloud uses to determine if a change to a file or directory matches a custom start condition.

`mode`

`string`

A string that indicates whether a workflow’s start condition’s Files and Folders setting should start a new build or not for a change.

Possible Values: `START_IF_ANY_FILE_MATCHES, DO_NOT_START_IF_ALL_FILES_MATCH`

## Topics

### Objects

object CiStartConditionFileMatcher

The data structure that represents a Start Condition File Matchers resource.

## See Also

### Objects

object CiBranchStartCondition

Settings for a start condition that starts a build if a branch changes.

object CiTagStartCondition

Settings for a start condition that starts a build if a Git tag changes.

object CiPullRequestStartCondition

Settings for a start condition that starts a build if a pull request changes.

object CiScheduledStartCondition

Settings for a start condition that starts a build based on a schedule.

