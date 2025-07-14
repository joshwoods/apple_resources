

- AppKit
- NSRunningApplication
-  current 

Type Property

# current

Returns an `NSRunningApplication` representing this application.

macOS 10.6+

``` source
class var current: NSRunningApplication { get }
```

## Return Value

An `NSRunningApplication` instance for the current application.

## See Also

### Getting running application instances

convenience init?(processIdentifier: pid_t)

Returns the running application with the given process identifier, or nil if no application has that pid.

class func runningApplications(withBundleIdentifier: String) -> [NSRunningApplication]

Returns an array of currently running applications with the specified bundle identifier.

