

- Foundation
- NSValue
-  pointerValue 

Instance Property

# pointerValue

Returns the value as an untyped pointer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var pointerValue: UnsafeMutableRawPointer? { get }
```

## Return Value

The value as a pointer to void. If the value object was not created to hold a pointer-sized data item, the result is undefined.

## See Also

### Working with Pointer and Object Values

init(pointer: UnsafeRawPointer?)

Creates a value object containing the specified pointer.

init(nonretainedObject: Any?)

Creates a value object containing the specified object.

var nonretainedObjectValue: Any?

The value as a non-retained pointer to an object.

