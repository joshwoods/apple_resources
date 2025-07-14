

- Foundation
- NSPointerFunctions
-  isEqualFunction 

Instance Property

# isEqualFunction

The function used to compare pointers.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isEqualFunction: ((UnsafeRawPointer, UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> ObjCBool)? { get set }
```

## See Also

### Personality Functions

var hashFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Int)?

The hash function.

var sizeFunction: ((UnsafeRawPointer) -> Int)?

The function used to determine the size of pointers.

var descriptionFunction: ((UnsafeRawPointer) -> String?)?

