

- HomeKit
- HMError
-  cannotRemoveBuiltinActionSet 

Type Property

# cannotRemoveBuiltinActionSet

An error indicating the built-in action set cannot be removed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var cannotRemoveBuiltinActionSet: HMError.Code { get }
```

## See Also

### Detecting action set errors

static var actionInAnotherActionSet: HMError.Code

An attempt to add an action that exists in one action set to another action set.

static var actionSetExecutionFailed: HMError.Code

An attempt to execute the action set failed.

static var actionSetExecutionInProgress: HMError.Code

An error indicating the execution of the action set is in progress.

static var actionSetExecutionPartialSuccess: HMError.Code

An attempt to execute the action set was only partially successful.

static var noActionsInActionSet: HMError.Code

An attempt to execute an action set with no actions.

static var noRegisteredActionSets: HMError.Code

An attempt to activate a trigger with no action sets.

