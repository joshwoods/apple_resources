

- App Store Connect API
-  CiScheduledStartCondition 

Object

# CiScheduledStartCondition

Settings for a start condition that starts a build based on a schedule.

App Store Connect API 1.5+

``` source
object CiScheduledStartCondition
```

## Properties

`schedule`

CiScheduledStartCondition.Schedule

The schedule information you configure for a workflow that starts a new build based on a schedule.

`source`

CiBranchPatterns

The source branch name and custom patterns you configure for a workflow that starts a new build on a schedule.

## Topics

### Objects

object CiScheduledStartCondition.Schedule

The schedule of an Xcode Cloud workflow that starts a new build based on a schedule.

## See Also

### Objects

object CiBranchStartCondition

Settings for a start condition that starts a build if a branch changes.

object CiTagStartCondition

Settings for a start condition that starts a build if a Git tag changes.

object CiPullRequestStartCondition

Settings for a start condition that starts a build if a pull request changes.

object CiFilesAndFoldersRule

Settings Xcode Cloud uses to determine whether a change should start a new build or not.

