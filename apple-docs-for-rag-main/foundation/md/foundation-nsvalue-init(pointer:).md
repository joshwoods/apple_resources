

- Foundation
- NSValue
-  init(pointer:) 

Initializer

# init(pointer:)

Creates a value object containing the specified pointer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(pointer: UnsafeRawPointer?)
```

## Parameters 

`pointer`  

The value for the new object.

## Return Value

A new value object that contains `aPointer`.

## Discussion

This method is equivalent to invoking init(_:withObjCType:) in this manner:

```
NSValue *theValue = [NSValue value:&aPointer withObjCType:@encode(void *)];
```

This method does not copy the contents of `aPointer`, so you must not to free the memory at the pointer destination while the NSValue object exists. NSData objects may be more suited for arbitrary pointers than NSValue objects.

## See Also

### Working with Pointer and Object Values

init(nonretainedObject: Any?)

Creates a value object containing the specified object.

var pointerValue: UnsafeMutableRawPointer?

Returns the value as an untyped pointer.

var nonretainedObjectValue: Any?

The value as a non-retained pointer to an object.

