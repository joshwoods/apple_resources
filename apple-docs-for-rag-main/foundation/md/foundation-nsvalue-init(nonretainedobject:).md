

- Foundation
- NSValue
-  init(nonretainedObject:) 

Initializer

# init(nonretainedObject:)

Creates a value object containing the specified object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(nonretainedObject anObject: Any?)
```

## Parameters 

`anObject`  

The value for the new object.

## Return Value

A new value object that contains `anObject`.

## Discussion

This method is equivalent to invoking init(_:withObjCType:) in this manner:

```
NSValue *theValue = [NSValue value:&anObject withObjCType:@encode(void *)];
```

This method is useful if you want to add an object to a Collection but don’t want the collection to create a strong reference to it.

## See Also

### Working with Pointer and Object Values

init(pointer: UnsafeRawPointer?)

Creates a value object containing the specified pointer.

var pointerValue: UnsafeMutableRawPointer?

Returns the value as an untyped pointer.

var nonretainedObjectValue: Any?

The value as a non-retained pointer to an object.

