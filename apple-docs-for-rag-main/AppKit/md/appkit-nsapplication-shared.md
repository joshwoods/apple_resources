

- AppKit
- NSApplication
-  shared 

Type Property

# shared

Returns the application instance, creating it if it doesn’t exist yet.

macOS

``` source
@MainActor
class var shared: NSApplication { get }
```

## Return Value

The shared application object.

## Mentioned in 

Passing control from one app to another with cooperative activation

## Discussion

This method also makes a connection to the window server and completes other initialization. Your program should invoke this method as one of the first statements in `main()`; this invoking is done for you if you create your application with Xcode. To retrieve the `NSApplication` instance after it has been created, use the global variable NSApp or invoke this method.

## See Also

### Related Documentation

Mac App Programming Guide

func run()

Starts the main event loop.

func terminate(Any?)

Terminates the receiver.

### Getting the Shared App Object

var NSApp: NSApplication!

The global variable for the shared app instance.

