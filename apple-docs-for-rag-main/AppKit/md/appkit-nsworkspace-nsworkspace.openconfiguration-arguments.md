

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  arguments 

Instance Property

# arguments

The set of command-line arguments to pass to a new app instance at launch time.

macOS 10.15+

``` source
var arguments: [String] { get set }
```

## Discussion

The default value of this property is an empty array. When launching a new instance of an app, use this property to specify any additional launch arguments. The system inserts the app’s path as the first element in the array.

If the calling process is sandboxed, the system ignores the value of this property.

## See Also

### Specifying Launch Attributes

var appleEvent: NSAppleEventDescriptor?

The first Apple event to send to the new app.

var environment: [String : String]

The set of environment variables to set in a new app instance.

var architecture: cpu_type_t

The architecture version of the app to launch.

