

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  architecture 

Instance Property

# architecture

The architecture version of the app to launch.

macOS 10.15+

``` source
var architecture: cpu_type_t { get set }
```

## Discussion

The default value of this property is `CPU_TYPE_ANY`, which causes the system to launch the app’s preferred architecture. You may specify a different value to force the system to launch that architecture. For a list of possible types, see the `` header file.

## See Also

### Specifying Launch Attributes

var appleEvent: NSAppleEventDescriptor?

The first Apple event to send to the new app.

var arguments: [String]

The set of command-line arguments to pass to a new app instance at launch time.

var environment: [String : String]

The set of environment variables to set in a new app instance.

