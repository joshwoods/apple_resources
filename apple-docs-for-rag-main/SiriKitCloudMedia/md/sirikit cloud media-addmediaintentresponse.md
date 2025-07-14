

- SiriKit Cloud Media
-  AddMediaIntentResponse 

Object

# AddMediaIntentResponse

A structure that contains a response code indicating your service’s progress in handling an add media intent.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaIntentResponse
```

## Properties

`class`

`string`

 (Required) 

The specific type of response.

Value: `AddMediaIntentResponse`

`code`

AddMediaIntentResponseCode

 (Required) 

A response code that indicates whether your service can add the media items to the library or playlist.

## Relationships

### Inherits From

- IntentResponse

## See Also

### Confirming and Handling an Add Media Intent

type AddMediaIntentResponseCode

Codes your service can return when confirming or handling an add media intent.

object AddMediaIntentHandlingConfirmInvocationResponse

The service’s response to a request to confirm an add media intent.

object AddMediaIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved add media intent.

