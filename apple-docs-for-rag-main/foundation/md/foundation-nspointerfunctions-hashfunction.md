

- Foundation
- NSPointerFunctions
-  hashFunction 

Instance Property

# hashFunction

The hash function.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hashFunction: ((UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> Int)? { get set }
```

## See Also

### Personality Functions

var isEqualFunction: ((UnsafeRawPointer, UnsafeRawPointer, ((UnsafeRawPointer) -> Int)?) -> ObjCBool)?

The function used to compare pointers.

var sizeFunction: ((UnsafeRawPointer) -> Int)?

The function used to determine the size of pointers.

var descriptionFunction: ((UnsafeRawPointer) -> String?)?

