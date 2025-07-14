

- Foundation
- Bundle
-  allFrameworks 

Type Property

# allFrameworks

Returns an array of all of the application’s bundles that represent frameworks.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var allFrameworks: [Bundle] { get }
```

## Return Value

An array of all of the application’s bundles that represent frameworks. Only frameworks with one or more Objective-C classes in them are included.

## Discussion

The returned array includes frameworks that are linked into an application when the application is built and bundles for frameworks that have been dynamically created.

## See Also

### Getting Standard Bundle Objects

class var main: Bundle

Returns the bundle object that contains the current executable.

class var allBundles: [Bundle]

Returns an array of all the application’s non-framework bundles.

