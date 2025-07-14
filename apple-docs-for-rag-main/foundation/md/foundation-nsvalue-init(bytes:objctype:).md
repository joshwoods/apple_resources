

- Foundation
- NSValue
-  init(bytes:objCType:) 

Initializer

# init(bytes:objCType:)

Initializes a value object to contain the specified value, interpreted with the specified Objective-C type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    bytes value: UnsafeRawPointer,
    objCType type: UnsafePointer
)
```

## Parameters 

`value`  

A pointer to data to be stored in the new value object.

`type`  

The Objective-C type of `value`, as provided by the `@encode()` compiler directive. Do not hard-code this parameter as a C string.

## Return Value

An initialized value object that contains `value`, which is interpreted as being of the Objective-C type `type`. The returned object might be different than the original receiver.

## Discussion

See Number and Value Programming Topics for other considerations in creating a value object.

This is the designated initializer for the NSValue class.

## See Also

### Related Documentation

Number and Value Programming Topics

### Working with Raw Values

init(UnsafeRawPointer, withObjCType: UnsafePointer&lt;CChar>)

Creates a value object containing the specified value, interpreted with the specified Objective-C type.

func getValue(UnsafeMutableRawPointer)

Copies the value into the specified buffer.

var objCType: UnsafePointer&lt;CChar>

A C string containing the Objective-C type of the data contained in the value object.

