

- App Store Connect API
- CiWorkflowCreateRequest
- CiWorkflowCreateRequest.Data
-  CiWorkflowCreateRequest.Data.Attributes 

Object

# CiWorkflowCreateRequest.Data.Attributes

The attributes you set that describe the new Xcode Cloud workflow resource.

App Store Connect API 1.5+

``` source
object CiWorkflowCreateRequest.Data.Attributes
```

## Properties

`actions`

`[`CiAction`]`

 (Required) 

The workflow’s actions.

`clean`

`boolean`

 (Required) 

A Boolean value that indicates whether Xcode Cloud should perform a clean build.

`containerFilePath`

`string`

 (Required) 

The relative path to your Xcode project or workspace.

`description`

`string`

 (Required) 

The workflow description.

`isEnabled`

`boolean`

 (Required) 

A Boolean value that indicates whether the workflow is active or deactivated.

`name`

`string`

 (Required) 

The name of the workflow you want to create; for example, `My New Workflow`.

`isLockedForEditing`

`boolean`

A Boolean value that indicates whether edits to the workflow are restricted.

`pullRequestStartCondition`

CiPullRequestStartCondition

A start condition that starts new builds for changes to a pull request.

`scheduledStartCondition`

CiScheduledStartCondition

A start condition that starts new builds based on a custom schedule.

`branchStartCondition`

CiBranchStartCondition

A start condition that starts new builds for changes to a branch.

`tagStartCondition`

CiTagStartCondition

A start condition that starts new builds for changes to a tag.

`manualBranchStartCondition`

CiManualBranchStartCondition

`manualPullRequestStartCondition`

CiManualPullRequestStartCondition

`manualTagStartCondition`

CiManualTagStartCondition

## See Also

### Objects

object CiWorkflowCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

