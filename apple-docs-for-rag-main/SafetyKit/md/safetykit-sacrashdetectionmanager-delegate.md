

- SafetyKit
- SACrashDetectionManager
-  delegate 

Instance Property

# delegate

The object that receives Crash Detection events.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
weak var delegate: (any SACrashDetectionDelegate)? { get set }
```

## See Also

### Requesting authorization

func requestAuthorization(completionHandler: (SAAuthorizationStatus, (any Error)?) -> Void)

Requests permission to access Crash Detection information.

