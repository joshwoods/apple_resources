

- Scripting Bridge
- SBApplication
-  isRunning 

Instance Property

# isRunning

A Boolean that indicates whether the target application represented by the receiver is running.

Mac Catalyst 13.0+macOS 10.5+

``` source
var isRunning: Bool { get }
```

## Discussion

true if the application is running, false otherwise.

This may be true for instances initialized with a bundle identifier or URL because `SBApplication` launches the application only when it’s necessary to send it an event.

## See Also

### Controlling the Application

func activate()

Moves the target application to the foreground immediately.

var launchFlags: LSLaunchFlags

The launch flags for the application represented by the receiver.

var sendMode: AESendMode

The mode for sending Apple events to the target application.

var timeout: Int

The period the application will wait to receive reply Apple events.

