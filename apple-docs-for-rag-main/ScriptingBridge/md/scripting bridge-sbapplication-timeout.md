

- Scripting Bridge
- SBApplication
-  timeout 

Instance Property

# timeout

The period the application will wait to receive reply Apple events.

Mac Catalyst 13.0+macOS 10.5+

``` source
var timeout: Int { get set }
```

## Discussion

For more information, see Apple Event Manager.

The default timeout value is kAEDefaultTimeout, which is about a minute. If you want the receiver to wait indefinitely for reply Apple events, use kNoTimeOut. For more information, see Apple Event Manager.

## See Also

### Controlling the Application

func activate()

Moves the target application to the foreground immediately.

var isRunning: Bool

A Boolean that indicates whether the target application represented by the receiver is running.

var launchFlags: LSLaunchFlags

The launch flags for the application represented by the receiver.

var sendMode: AESendMode

The mode for sending Apple events to the target application.

