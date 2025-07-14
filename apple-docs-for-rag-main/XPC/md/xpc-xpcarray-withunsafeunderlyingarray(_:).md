

- XPC
- XPCArray
-  withUnsafeUnderlyingArray(\_:) 

Instance Method

# withUnsafeUnderlyingArray(\_:)

Calls a closure with an unsafe reference to the array.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
func withUnsafeUnderlyingArray(_ closure: (xpc_object_t) throws -> ReturnType) rethrows -> ReturnType
```

## Parameters 

`closure`  

A closure that takes an xpc_object_t parameter. If `closure` has a return value, that value is also used as the return value for the withUnsafeUnderlyingArray(body:) function.

## Return Value

The return value, if any, of the closure.

## See Also

### Accessing elements

subscript(Int) -> XPCDictionary?

Reads and writes the value at the given index as an XPC dictionary.

subscript(Int) -> String?

Reads and writes the value at the given index as a string.

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

