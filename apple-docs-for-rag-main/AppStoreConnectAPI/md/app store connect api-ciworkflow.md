

- App Store Connect API
-  CiWorkflow 

Object

# CiWorkflow

The data structure that represents a Workflows resource.

App Store Connect API 1.5+

``` source
object CiWorkflow
```

## Properties

`attributes`

CiWorkflow.Attributes

The attributes that describe the Workflows resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a Workflows resource.

`links`

ResourceLinks

The navigational links that include the self-link.

`relationships`

CiWorkflow.Relationships

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `ciWorkflows`

## Topics

### Objects

object CiWorkflow.Attributes

The attributes that describe a Workflows resource.

object CiWorkflow.Relationships

The relationships of the Workflows resource you included in the request and those on which you can operate.

## See Also

### Objects and Types

object CiAction

The data structure that represents an Xcode Cloud workflow action resource.

object CiWorkflowCreateRequest

The request body you use to create a new Xcode Cloud workflow.

object CiWorkflowUpdateRequest

The request body you use to update an Xcode Cloud workflow.

object CiWorkflowResponse

A response that contains a single Workflows resource.

object CiWorkflowsResponse

A response that contains a list of Workflows resources.

object CiBuildRunsResponse

A response that contains a list of Build Runs resources.

object CiManualBranchStartCondition

object CiManualPullRequestStartCondition

object CiManualTagStartCondition

