

- SiriKit Cloud Media
-  Intent 

Object

# Intent

A user request for your service to fulfill.

SiriKit Cloud Media 1.0.2+

``` source
object Intent
```

## Properties

`class`

`string`

 (Required) 

The specific type of intent.

`identifier`

`string`

 (Required) 

The unique identifier for this intent object.

## Relationships

### Inherited By

- AddMediaIntent
- PlayMediaIntent
- UpdateMediaAffinityIntent

## See Also

### Intents

object IntentResponse

Your service’s response to an intent.

object UserActivity

The context for playing a media queue.

object IntentResolutionResult

An object that matches a parameter of an intent, or information about why your service can’t determine a value for the parameter.

object BooleanResolutionResult

A Boolean value that matches an intent parameter, or information about why your service can’t determine the value.

