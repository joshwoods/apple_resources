

- SiriKit Cloud Media
-  AddMediaIntentHandlingConfirmInvocationResponse 

Object

# AddMediaIntentHandlingConfirmInvocationResponse

The service’s response to a request to confirm an add media intent.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaIntentHandlingConfirmInvocationResponse
```

## Properties

`result`

AddMediaIntentHandlingConfirmInvocationResponse.Result

 (Required) 

The results of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `AddMediaIntentHandling.confirm`

## Topics

### Specifying the Result

object AddMediaIntentHandlingConfirmInvocationResponse.Result

The result of receiving the user’s confirmation that they want to add the media items to the destination.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Confirming and Handling an Add Media Intent

object AddMediaIntentResponse

A structure that contains a response code indicating your service’s progress in handling an add media intent.

type AddMediaIntentResponseCode

Codes your service can return when confirming or handling an add media intent.

object AddMediaIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved add media intent.

