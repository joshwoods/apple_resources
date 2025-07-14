

- SiriKit Cloud Media
-  IntentResponse 

Object

# IntentResponse

Your service’s response to an intent.

SiriKit Cloud Media 1.0.2+

``` source
object IntentResponse
```

## Properties

`class`

`string`

 (Required) 

The specific type of response.

`userActivity`

UserActivity

 (Required) 

A description of the interaction in progress.

## Relationships

### Inherited By

- AddMediaIntentResponse
- PlayMediaIntentResponse
- UpdateMediaAffinityIntentResponse

## See Also

### Intents

object Intent

A user request for your service to fulfill.

object UserActivity

The context for playing a media queue.

object IntentResolutionResult

An object that matches a parameter of an intent, or information about why your service can’t determine a value for the parameter.

object BooleanResolutionResult

A Boolean value that matches an intent parameter, or information about why your service can’t determine the value.

