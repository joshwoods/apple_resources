

- SiriKit Cloud Media
-  UserActivity 

Object

# UserActivity

The context for playing a media queue.

SiriKit Cloud Media 1.0.2+

``` source
object UserActivity
```

## Properties

`activityType`

`string`

 (Required) 

A reverse-DNS string that uniquely identifies the activity. Provide the same activity types your app specifies in NSUserActivity objects.

Maximum length: `250`

`persistentIdentifier`

`string`

An identifier for this activity.

Maximum length: `250`

`title`

`string`

A short description of this activity for logging or debugging purposes.

Maximum length: `250`

`userInfo`

UserActivity.UserActivityUserInfo

Additional data your service needs to fulfill requests to Get a Media Queue.

`version`

`string`

 (Required) 

The version of the `SiriKitMediaAPI` library this activity conforms to.

Maximum length: `25`

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

## Discussion

Create a `UserActivity` and provide it in your response to a Process a Play Media Intent. When the client receives your response, it includes this activity in its request to Get a Media Queue to define the queue it’s requesting.

## Topics

### Maintaining State

object UserActivity.UserActivityUserInfo

A dictionary that contains service-specific state information necessary to continue an activity in a separate request.

## See Also

### Intents

object Intent

A user request for your service to fulfill.

object IntentResponse

Your service’s response to an intent.

object IntentResolutionResult

An object that matches a parameter of an intent, or information about why your service can’t determine a value for the parameter.

object BooleanResolutionResult

A Boolean value that matches an intent parameter, or information about why your service can’t determine the value.

