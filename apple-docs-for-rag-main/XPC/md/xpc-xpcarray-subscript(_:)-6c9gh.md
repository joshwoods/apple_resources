

- XPC
- XPCArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Reads and writes the value at the given index as a string.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
subscript(index: Int) -> String? { get set }
```

## Parameters 

`index`  

The position of the element to access.

## Return Value

The value at the specified index in the array, otherwise Nil.

## See Also

### Accessing elements

subscript(Int) -> XPCDictionary?

Reads and writes the value at the given index as an XPC dictionary.

subscript(Int) -> Bool?

Reads and writes the value at the given index as a Boolean value.

subscript(Int) -> xpc_object_t?

Reads and writes the value at the given index as an XPC object.

subscript&lt;T>(Int) -> T?

Reads and writes the value at the given index as a floating point value.

subscript&lt;T>(Int) -> T?

Reads and writes the value at the given index as an unsigned integer.

subscript&lt;T>(Int) -> T?

Reads and writes the value at the given index as a signed integer.

subscript(Int, as _: XPCDictionary.Type) -> XPCDictionary?

Reads the value associated with the given key as an XPC dictionary.

subscript(Int, as _: String.Type) -> String?

Reads and writes the value at the given index as a string.

subscript(Int, as _: Bool.Type) -> Bool?

Reads and writes the value at the given index as a Boolean value.

subscript(Int, as _: any OS_xpc_object.Type) -> xpc_object_t?

Reads and writes the value at the given index as an XPC object.

subscript(Int, as _: xpc_type_t) -> xpc_object_t?

Reads and writes the value at the given index as an XPC object.

subscript&lt;T>(Int, as _: T.Type) -> T?

Reads and writes the value at the given index as a floating point value.

subscript&lt;T>(Int, as _: T.Type) -> T?

Reads and writes the value at the given index as an integer value.

subscript(Int, as _: Bool.Type, default _: @autoclosure () -> Bool) -> Bool

Reads and writes the value at the given index as a Boolean value, falling back to the given default value.

subscript&lt;T>(Int, as _: T.Type, default _: @autoclosure () -> T) -> T

Reads and writes the value at the given index as a floating point value, falling back to the given default value.

