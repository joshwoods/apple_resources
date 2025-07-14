

- App Store Connect API
-  CiAction 

Object

# CiAction

The data structure that represents an Xcode Cloud workflow action resource.

App Store Connect API 1.5+

``` source
object CiAction
```

## Properties

`actionType`

CiActionType

The type of the action.

`buildDistributionAudience`

BuildAudienceType

A type that indicates whether a build’s artifact is eligible for release on the App Store.

`destination`

`string`

A string that describes the destination Xcode Cloud uses for an action.

Possible Values: `ANY_IOS_DEVICE, ANY_IOS_SIMULATOR, ANY_TVOS_DEVICE, ANY_TVOS_SIMULATOR, ANY_WATCHOS_DEVICE, ANY_WATCHOS_SIMULATOR, ANY_MAC, ANY_MAC_CATALYST, ANY_VISIONOS_DEVICE, ANY_VISIONOS_SIMULATOR`

`isRequiredToPass`

`boolean`

A Boolean value that indicates whether the action must succeed in order for a build to succeed.

`name`

`string`

The name of the action; for example, archive or test.

`platform`

`string`

The platform Xcode Cloud uses for the action.

Possible Values: `MACOS, IOS, TVOS, WATCHOS, VISIONOS`

`scheme`

`string`

The name of the scheme that Xcode Cloud uses to perform the action.

`testConfiguration`

CiAction.TestConfiguration

An action’s test configuration. Only set this field for test actions.

## Topics

### Objects

object CiAction.TestConfiguration

The test configuration for a test action.

## See Also

### Objects and Types

object CiWorkflow

The data structure that represents a Workflows resource.

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

