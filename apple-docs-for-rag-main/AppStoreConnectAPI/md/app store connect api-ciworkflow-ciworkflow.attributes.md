

- App Store Connect API
- CiWorkflow
-  CiWorkflow.Attributes 

Object

# CiWorkflow.Attributes

The attributes that describe a Workflows resource.

App Store Connect API 1.5+

``` source
object CiWorkflow.Attributes
```

## Properties

`actions`

`[`CiAction`]`

The actions that are part of the workflow.

`clean`

`boolean`

A Boolean value that indicates whether Xcode Cloud should perform a clean build.

`containerFilePath`

`string`

The relative path to your Xcode project or workspace.

`description`

`string`

The workflow’s description.

`isEnabled`

`boolean`

A Boolean value that indicates whether the workflow is active or deactivated.

`isLockedForEditing`

`boolean`

A Boolean value that indicates whether edits to the workflow are restricted.

`lastModifiedDate`

`date-time`

The date and time when the workflow was last modified.

`name`

`string`

The name of the Xcode Cloud workflow; for example, `My Workflow`.

`pullRequestStartCondition`

CiPullRequestStartCondition

The workflow’s start condition for pull request changes.

`scheduledStartCondition`

CiScheduledStartCondition

The workflow’s start condition that starts new builds on a custom schedule.

`branchStartCondition`

CiBranchStartCondition

The workflow’s start condition that starts new builds for changes to a branch.

`tagStartCondition`

CiTagStartCondition

The workflow’s start condition that starts new builds for changes to a tag.

`manualBranchStartCondition`

CiManualBranchStartCondition

`manualPullRequestStartCondition`

CiManualPullRequestStartCondition

`manualTagStartCondition`

CiManualTagStartCondition

## Topics

### Objects

object CiBranchStartCondition

Settings for a start condition that starts a build if a branch changes.

object CiTagStartCondition

Settings for a start condition that starts a build if a Git tag changes.

object CiPullRequestStartCondition

Settings for a start condition that starts a build if a pull request changes.

object CiScheduledStartCondition

Settings for a start condition that starts a build based on a schedule.

object CiFilesAndFoldersRule

Settings Xcode Cloud uses to determine whether a change should start a new build or not.

## See Also

### Objects

object CiWorkflow.Relationships

The relationships of the Workflows resource you included in the request and those on which you can operate.

