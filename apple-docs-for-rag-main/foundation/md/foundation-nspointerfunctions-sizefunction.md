

- Foundation
- NSPointerFunctions
-  sizeFunction 

Instance Property

# sizeFunction

The function used to determine the size of pointers.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var sizeFunction: ((UnsafeRawPointer) -> Int)? { get set }
```

## Discussion

This function is used for copy-in operations (unless the collection has an object personality).

## See Also

### Personality Functions

var hashFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Int)?

The hash function.

var isEqualFunction: ((UnsafeRawPointer, UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> ObjCBool)?

The function used to compare pointers.

var descriptionFunction: ((UnsafeRawPointer) -> String?)?

