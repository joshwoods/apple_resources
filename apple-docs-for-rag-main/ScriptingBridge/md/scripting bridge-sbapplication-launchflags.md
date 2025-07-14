

- Scripting Bridge
- SBApplication
-  launchFlags 

Instance Property

# launchFlags

The launch flags for the application represented by the receiver.

Mac Catalyst 13.0+macOS 10.5+

``` source
var launchFlags: LSLaunchFlags { get set }
```

## Discussion

For more information, see Launch Services.

## See Also

### Controlling the Application

func activate()

Moves the target application to the foreground immediately.

var isRunning: Bool

A Boolean that indicates whether the target application represented by the receiver is running.

var sendMode: AESendMode

The mode for sending Apple events to the target application.

var timeout: Int

The period the application will wait to receive reply Apple events.

