

- Core Motion
- CMHeadphoneActivityManager
-  CMHeadphoneActivityManager.StatusHandler 

Type Alias

# CMHeadphoneActivityManager.StatusHandler

The type for a handler to be invoked with status updates.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+watchOS 2.0+

``` source
typealias StatusHandler = (CMHeadphoneActivityManager.Status, (any Error)?) -> Void
```

## See Also

### Supporting Types

enum Status

Headphone connection status updates.

typealias ActivityHandler

The type for a handler to be invoked when headphone motion activity data is available.

