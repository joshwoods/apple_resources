

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  environment 

Instance Property

# environment

The set of environment variables to set in a new app instance.

macOS 10.15+

``` source
var environment: [String : String] { get set }
```

## Discussion

The default value of this property is an empty dictionary. When launching a new instance of an app, use this property to specify the key/value pairs for any environment variables.

If the calling process is sandboxed, the system ignores the value of this property.

## See Also

### Specifying Launch Attributes

var appleEvent: NSAppleEventDescriptor?

The first Apple event to send to the new app.

var arguments: [String]

The set of command-line arguments to pass to a new app instance at launch time.

var architecture: cpu_type_t

The architecture version of the app to launch.

