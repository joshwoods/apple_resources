

- AppKit
-  NSApp 

Global Variable

# NSApp

The global variable for the shared app instance.

macOS

``` source
@MainActor
var NSApp: NSApplication!
```

## Discussion

The value in this global variable is the same as accessing the shared property of the app.

## See Also

### Getting the Shared App Object

class var shared: NSApplication

Returns the application instance, creating it if it doesn’t exist yet.

