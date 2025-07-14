

- Core Motion
- CMFallDetectionManager
-  authorizationStatus 

Instance Property

# authorizationStatus

The authorization status for receiving fall detection event notifications.

watchOS 7.2+

``` source
var authorizationStatus: CMAuthorizationStatus { get }
```

## See Also

### Requesting Authorization

func requestAuthorization(handler: (CMAuthorizationStatus) -> Void)

Requests authorization to receive notifications about fall detection events.

enum CMAuthorizationStatus

The authorization status for motion-related features.

