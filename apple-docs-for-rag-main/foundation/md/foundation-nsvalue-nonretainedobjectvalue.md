

- Foundation
- NSValue
-  nonretainedObjectValue 

Instance Property

# nonretainedObjectValue

The value as a non-retained pointer to an object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var nonretainedObjectValue: Any? { get }
```

## Discussion

If the value was not created to hold a pointer-sized data item, the result is undefined.

## See Also

### Working with Pointer and Object Values

init(pointer: UnsafeRawPointer?)

Creates a value object containing the specified pointer.

init(nonretainedObject: Any?)

Creates a value object containing the specified object.

var pointerValue: UnsafeMutableRawPointer?

Returns the value as an untyped pointer.

