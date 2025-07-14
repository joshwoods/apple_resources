

- App Store Connect API
-  CiWorkflowResponse 

Object

# CiWorkflowResponse

A response that contains a single Workflows resource.

App Store Connect API 1.5+

``` source
object CiWorkflowResponse
```

## Properties

`data`

CiWorkflow

 (Required) 

The resource data.

`included`

`[*]`

The requested relationship data.

Possible types: CiProduct`, `ScmRepository`, `CiXcodeVersion`, `CiMacOsVersion

`links`

DocumentLinks

 (Required) 

The navigational links that include the self-link.

## See Also

### Objects and Types

object CiWorkflow

The data structure that represents a Workflows resource.

object CiAction

The data structure that represents an Xcode Cloud workflow action resource.

object CiWorkflowCreateRequest

The request body you use to create a new Xcode Cloud workflow.

object CiWorkflowUpdateRequest

The request body you use to update an Xcode Cloud workflow.

object CiWorkflowsResponse

A response that contains a list of Workflows resources.

object CiBuildRunsResponse

A response that contains a list of Build Runs resources.

object CiManualBranchStartCondition

object CiManualPullRequestStartCondition

object CiManualTagStartCondition

