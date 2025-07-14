

- Core Motion
- CMMovementDisorderManager
-  authorizationStatus() 

Type Method

# authorizationStatus()

A value indicating whether the user has authorized the app to monitor and query for movement disorder data.

watchOS 5.0+

``` source
class func authorizationStatus() -> CMAuthorizationStatus
```

## Discussion

The first time your app attempts to monitor or query for movement disorder data, the manager asks the user for permission to collect or retrieve their movement disorder data. To request permission, your app must set a motion usage description in its `Info.plist` file. For more information, see Provide the motion usage description.

## See Also

### Checking Availablility

class func isAvailable() -> Bool

A Boolean value indicating whether the current device supports the movement disorder manager.

class func version() -> String?

Returns a string that describes the movement disorder algorithm’s current version.

