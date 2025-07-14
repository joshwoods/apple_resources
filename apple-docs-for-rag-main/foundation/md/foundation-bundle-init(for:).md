

- Foundation
- Bundle
-  init(for:) 

Initializer

# init(for:)

Returns the `NSBundle` object with which the specified class is associated.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(for aClass: AnyClass)
```

## Parameters 

`aClass`  

A class.

## Return Value

The `NSBundle` object that dynamically loaded `aClass` (a loadable bundle), the `NSBundle` object for the framework in which `aClass` is defined, or the main bundle object if `aClass` was not dynamically loaded or is not defined in a framework.

## Discussion

This method creates and returns a new `NSBundle` object if there is no existing bundle associated with `aClass`. Otherwise, the existing instance is returned.

## See Also

### Related Documentation

class var main: Bundle

Returns the bundle object that contains the current executable.

### Creating and Initializing a Bundle

init?(identifier: String)

Returns the `NSBundle` instance that has the specified bundle identifier.

convenience init?(url: URL)

Returns an `NSBundle` object initialized to correspond to the specified file URL.

init?(path: String)

Returns an `NSBundle` object initialized to correspond to the specified directory.

