

- Foundation
- Bundle
-  main 

Type Property

# main

Returns the bundle object that contains the current executable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var main: Bundle { get }
```

## Return Value

The `NSBundle` object corresponding to the bundle directory that contains the current executable. This method may return a valid bundle object even for unbundled apps. It may also return `nil` if the bundle object could not be created, so always check the return value.

## Discussion

The main bundle lets you access the resources in the same directory as the currently running executable. For a running app, the main bundle offers access to the app’s bundle directory. For code running in a framework, the main bundle offers access to the framework’s bundle directory.

## See Also

### Related Documentation

Resource Programming Guide

init(for: AnyClass)

Returns the `NSBundle` object with which the specified class is associated.

Bundle Programming Guide

### Getting Standard Bundle Objects

class var allFrameworks: [Bundle]

Returns an array of all of the application’s bundles that represent frameworks.

class var allBundles: [Bundle]

Returns an array of all the application’s non-framework bundles.

