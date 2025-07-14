

- AppKit
- NSUserDefaultsController
-  shared 

Type Property

# shared

Returns the shared instance of NSUserDefaultsController, creating it if necessary.

macOS

``` source
class var shared: NSUserDefaultsController { get }
```

## Discussion

This instance has no initial values, and uses `[NSUserDefaults standardUserDefaults]` to create the defaults. An application can get this object when an application launches and configure it as required.

## See Also

### Related Documentation

Cocoa Bindings Programming Topics

