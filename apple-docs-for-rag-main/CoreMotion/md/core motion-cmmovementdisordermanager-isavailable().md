

- Core Motion
- CMMovementDisorderManager
-  isAvailable() 

Type Method

# isAvailable()

A Boolean value indicating whether the current device supports the movement disorder manager.

watchOS 5.0+

``` source
class func isAvailable() -> Bool
```

## See Also

### Checking Availablility

class func authorizationStatus() -> CMAuthorizationStatus

A value indicating whether the user has authorized the app to monitor and query for movement disorder data.

class func version() -> String?

Returns a string that describes the movement disorder algorithm’s current version.

