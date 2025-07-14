

- Core Motion
- CMFallDetectionEvent
-  resolution 

Instance Property

# resolution

The event’s resolution.

watchOS 7.2+

``` source
var resolution: CMFallDetectionEvent.UserResolution { get }
```

## Discussion

The resolution of an event reflects the user’s action in response to the fall detection notification. For example, the user might tap a button to respond inside the notification, or press the digital crown to dismiss the notification.

## See Also

### Accessing Fall Data

enum UserResolution

User resolutions for fall detection events.

