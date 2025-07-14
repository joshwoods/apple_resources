

- AppKit
- NSRunningApplication
-  runningApplications(withBundleIdentifier:) 

Type Method

# runningApplications(withBundleIdentifier:)

Returns an array of currently running applications with the specified bundle identifier.

macOS 10.6+

``` source
class func runningApplications(withBundleIdentifier bundleIdentifier: String) -> [NSRunningApplication]
```

## Parameters 

`bundleIdentifier`  

The bundle identifier.

## Return Value

An array of `NSRunningApplications`, or an empty array if no applications match the bundle identifier.

## Mentioned in 

Passing control from one app to another with cooperative activation

## See Also

### Getting running application instances

convenience init?(processIdentifier: pid_t)

Returns the running application with the given process identifier, or nil if no application has that pid.

class var current: NSRunningApplication

Returns an `NSRunningApplication` representing this application.

