

- SiriKit Cloud Media
-  AddMediaIntentResponseCode 

Type

# AddMediaIntentResponseCode

Codes your service can return when confirming or handling an add media intent.

SiriKit Cloud Media 1.0.2+

``` source
string AddMediaIntentResponseCode
```

## Possible Values 

`success`  

Your service successfully adds the media items to the specified destination. Use this in an AddMediaIntentHandlingHandleInvocationResponse.Result.

`ready`  

Your service is ready and able to add the media items to the specified destination. Use this in an AddMediaIntentHandlingConfirmInvocationResponse.Result.

`inProgress`  

Your service is adding the media items to the specified destination, but it may take some time. Use this in an AddMediaIntentHandlingHandleInvocationResponse.Result.

`failureRequiringAppLaunch`  

The user needs to launch your app on their iOS device to resolve a problem.

`failure`  

A failure occurs while confirming or handling the intent.

`unspecified`  

An unspecified response code.

## See Also

### Confirming and Handling an Add Media Intent

object AddMediaIntentResponse

A structure that contains a response code indicating your service’s progress in handling an add media intent.

object AddMediaIntentHandlingConfirmInvocationResponse

The service’s response to a request to confirm an add media intent.

object AddMediaIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved add media intent.

