

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  appleEvent 

Instance Property

# appleEvent

The first Apple event to send to the new app.

macOS 10.15+

``` source
var appleEvent: NSAppleEventDescriptor? { get set }
```

## Discussion

The default value of this property is `nil`, which causes the system to send a default Apple event, as needed. The system sends the event only if an instance of the app is already running.

## See Also

### Specifying Launch Attributes

var arguments: [String]

The set of command-line arguments to pass to a new app instance at launch time.

var environment: [String : String]

The set of environment variables to set in a new app instance.

var architecture: cpu_type_t

The architecture version of the app to launch.

