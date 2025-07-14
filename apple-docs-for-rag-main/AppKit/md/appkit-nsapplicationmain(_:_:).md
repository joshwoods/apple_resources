

- AppKit
-  NSApplicationMain(\_:\_:) 

Function

# NSApplicationMain(\_:\_:)

Called by the main function to create and run the application.

macOS 10.9+

``` source
func NSApplicationMain(
    _ argc: Int32,
    _ argv: UnsafeMutablePointer?>
) -> Int32
```

## Parameters 

`argc`  

The number of arguments in the `argv` parameter.

`argv`  

An array of pointers containing the arguments passed to the application at startup.

## Return Value

This method never returns a result code. Instead, it calls the `exit` function to exit the application and terminate the process. If you want to determine why the application exited, you should look at the result code from the `exit` function instead.

## Discussion

Creates the application, loads the main nib file from the application’s main bundle, and runs the application. You must call this function from the main thread of your application, and you typically call it only once from your application’s `main` function. Your `main` function is usually generated automatically by Xcode.

### Special Considerations

`NSApplicationMain` itself ignores the `argc` and `argv` arguments. Instead, Cocoa gets its arguments indirectly through `_NSGetArgv`, `_NSGetArgc`, and `_NSGetEnviron` (see \).

## See Also

### Life Cycle

class NSApplication

An object that manages an app’s main event loop and resources used by all of that app’s objects.

class NSRunningApplication

An object that can manipulate and provide information for a single instance of an app.

protocol NSApplicationDelegate

A set of methods that manage your app’s life cycle and its interaction with common system services.

