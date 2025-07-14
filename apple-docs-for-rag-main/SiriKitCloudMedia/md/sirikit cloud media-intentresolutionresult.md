

- SiriKit Cloud Media
-  IntentResolutionResult 

Object

# IntentResolutionResult

An object that matches a parameter of an intent, or information about why your service can’t determine a value for the parameter.

SiriKit Cloud Media 1.0.2+

``` source
object IntentResolutionResult
```

## Properties

`class`

`string`

 (Required) 

The specific type of result.

`needsValue`

IntentResolutionResult.NeedsValue

The service must have a value for this parameter, but the intent doesn’t include one.

`notRequired`

IntentResolutionResult.NotRequired

The intent doesn’t include a value for this parameter, but the server can proceed without one.

`unsupported`

IntentResolutionResult.Unsupported

The server doesn’t support this parameter.

## Topics

### Providing a Generic Result

object IntentResolutionResult.NeedsValue

An empty object that indicates the service must have a value for this parameter, but the intent doesn’t include one.

object IntentResolutionResult.NotRequired

An empty object that indicates the intent doesn’t include a value for this parameter, but the server can proceed without one.

object IntentResolutionResult.Unsupported

An empty object that indicates the server doesn’t support this parameter.

## Relationships

### Inherited By

- AddMediaMediaDestinationResolutionResult
- AddMediaMediaItemResolutionResult
- BooleanResolutionResult
- MediaAffinityTypeResolutionResult
- PlayMediaMediaItemResolutionResult
- PlaybackQueueLocationResolutionResult
- PlaybackRepeatModeResolutionResult
- UpdateMediaAffinityMediaItemResolutionResult

## See Also

### Intents

object Intent

A user request for your service to fulfill.

object IntentResponse

Your service’s response to an intent.

object UserActivity

The context for playing a media queue.

object BooleanResolutionResult

A Boolean value that matches an intent parameter, or information about why your service can’t determine the value.

