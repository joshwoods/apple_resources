

- Foundation
- NSValue
-  init(\_:withObjCType:) 

Initializer

# init(\_:withObjCType:)

Creates a value object containing the specified value, interpreted with the specified Objective-C type.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    _ value: UnsafeRawPointer,
    withObjCType type: UnsafePointer
)
```

## Parameters 

`value`  

A pointer to data to be stored in the new value object.

`type`  

The Objective-C type of `value`, as provided by the `@encode()` compiler directive. Do not hard-code this parameter as a C string.

## Return Value

A new value object that contains `value`, which is interpreted as being of the Objective-C type `type`.

## Discussion

This method has the same effect as valueWithBytes:objCType: and may be deprecated in a future release. You should use valueWithBytes:objCType: instead.

## See Also

### Working with Raw Values

init(bytes: UnsafeRawPointer, objCType: UnsafePointer&lt;CChar>)

Initializes a value object to contain the specified value, interpreted with the specified Objective-C type.

func getValue(UnsafeMutableRawPointer)

Copies the value into the specified buffer.

var objCType: UnsafePointer&lt;CChar>

A C string containing the Objective-C type of the data contained in the value object.

