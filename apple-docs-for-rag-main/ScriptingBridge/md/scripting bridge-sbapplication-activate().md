

- Scripting Bridge
- SBApplication
-  activate() 

Instance Method

# activate()

Moves the target application to the foreground immediately.

Mac Catalyst 13.0+macOS 10.5+

``` source
func activate()
```

## Discussion

If the target application is not already running, this method launches it.

## See Also

### Controlling the Application

var isRunning: Bool

A Boolean that indicates whether the target application represented by the receiver is running.

var launchFlags: LSLaunchFlags

The launch flags for the application represented by the receiver.

var sendMode: AESendMode

The mode for sending Apple events to the target application.

var timeout: Int

The period the application will wait to receive reply Apple events.

