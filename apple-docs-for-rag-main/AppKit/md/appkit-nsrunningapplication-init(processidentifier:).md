

- AppKit
- NSRunningApplication
-  init(processIdentifier:) 

Initializer

# init(processIdentifier:)

Returns the running application with the given process identifier, or nil if no application has that pid.

macOS 10.6+

``` source
convenience init?(processIdentifier pid: pid_t)
```

## Parameters 

`pid`  

The process identifier.

## Return Value

An instance of `NSRunningApplication` for the specified `pid`, or nil if the application has no process identifier.

## Discussion

Applications that do not have `PIDs` cannot be returned from this method.

## See Also

### Getting running application instances

class func runningApplications(withBundleIdentifier: String) -> [NSRunningApplication]

Returns an array of currently running applications with the specified bundle identifier.

class var current: NSRunningApplication

Returns an `NSRunningApplication` representing this application.

