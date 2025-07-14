

- Foundation
- NSPointerFunctions
-  descriptionFunction 

Instance Property

# descriptionFunction

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var descriptionFunction: ((UnsafeRawPointer) -> String?)? { get set }
```

## See Also

### Personality Functions

var hashFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Int)?

The hash function.

var isEqualFunction: ((UnsafeRawPointer, UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> ObjCBool)?

The function used to compare pointers.

var sizeFunction: ((UnsafeRawPointer) -> Int)?

The function used to determine the size of pointers.

