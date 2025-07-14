

- Scripting Bridge
- SBApplication
-  sendMode 

Instance Property

# sendMode

The mode for sending Apple events to the target application.

Mac Catalyst 13.0+macOS 10.5+

``` source
var sendMode: AESendMode { get set }
```

## Discussion

For more information, see Apple Event Manager.

The default send mode is kAEWaitReply. If the send mode is something other than `kAEWaitReply`, the receiver might not correctly handle reply events from the target application.

## See Also

### Controlling the Application

func activate()

Moves the target application to the foreground immediately.

var isRunning: Bool

A Boolean that indicates whether the target application represented by the receiver is running.

var launchFlags: LSLaunchFlags

The launch flags for the application represented by the receiver.

var timeout: Int

The period the application will wait to receive reply Apple events.

