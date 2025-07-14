

- SiriKit Cloud Media
-  AddMediaIntentHandlingHandleInvocationResponse 

Object

# AddMediaIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved add media intent.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaIntentHandlingHandleInvocationResponse
```

## Properties

`result`

AddMediaIntentHandlingHandleInvocationResponse.Result

 (Required) 

The outcome of handling the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `AddMediaIntentHandling.handle`

## Topics

### Specifying the Result

object AddMediaIntentHandlingHandleInvocationResponse.Result

The result of handling an intent to add media items to a specified library or playlist.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Confirming and Handling an Add Media Intent

object AddMediaIntentResponse

A structure that contains a response code indicating your service’s progress in handling an add media intent.

type AddMediaIntentResponseCode

Codes your service can return when confirming or handling an add media intent.

object AddMediaIntentHandlingConfirmInvocationResponse

The service’s response to a request to confirm an add media intent.

