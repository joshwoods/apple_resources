

- SiriKit Cloud Media
-  BooleanResolutionResult 

Object

# BooleanResolutionResult

A Boolean value that matches an intent parameter, or information about why your service can’t determine the value.

SiriKit Cloud Media 1.0.2+

``` source
object BooleanResolutionResult
```

## Properties

`class`

`string`

The specific type of result.

Value: `BooleanResolutionResult`

`success`

BooleanResolutionResult.Success

A Boolean value that matches the intent.

`confirmationRequired`

BooleanResolutionResult.ConfirmationRequired

A Boolean value for the user to confirm or reject before proceeding.

## Discussion

Only provide one of the optional properties. If a client receives a result with more than one outcome, such as `needsValue` and `success`, it arbitrarily chooses one and ignores the rest.

## Topics

### Providing a Result

object BooleanResolutionResult.ConfirmationRequired

A result that requires the user to confirm the Boolean value before proceeding.

object BooleanResolutionResult.Success

A Boolean value that successfully matches the intent.

## Relationships

### Inherits From

- IntentResolutionResult

## See Also

### Intents

object Intent

A user request for your service to fulfill.

object IntentResponse

Your service’s response to an intent.

object UserActivity

The context for playing a media queue.

object IntentResolutionResult

An object that matches a parameter of an intent, or information about why your service can’t determine a value for the parameter.

