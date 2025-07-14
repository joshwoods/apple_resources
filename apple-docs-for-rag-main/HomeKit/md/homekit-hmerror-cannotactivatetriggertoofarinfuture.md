

- HomeKit
- HMError
-  cannotActivateTriggerTooFarInFuture 

Type Property

# cannotActivateTriggerTooFarInFuture

An error indicating the trigger cannot be activated because it is set too far in the future.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var cannotActivateTriggerTooFarInFuture: HMError.Code { get }
```

## See Also

### Detecting limit errors

static var dateMustBeOnSpecifiedBoundaries: HMError.Code

An error indicating the date is not on the specified boundaries.

static var fireDateInPast: HMError.Code

An attempt to activate a timer trigger with a date in the past.

static var invalidMessageSize: HMError.Code

An error indicating an invalid message size.

static var maximumObjectLimitReached: HMError.Code

An error indicating the maximum object count has been reached.

static var recurrenceTooLarge: HMError.Code

An attempt to use a recurrence period that is too large.

static var recurrenceTooSmall: HMError.Code

An error indicating the recurrence interval is too short.

static var recurrenceMustBeOnSpecifiedBoundaries: HMError.Code

An error indicating the recurrence rule is not on the specified boundaries.

