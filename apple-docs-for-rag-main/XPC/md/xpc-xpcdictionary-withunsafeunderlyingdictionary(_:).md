

- XPC
- XPCDictionary
-  withUnsafeUnderlyingDictionary(\_:) 

Instance Method

# withUnsafeUnderlyingDictionary(\_:)

Calls a closure with an unsafe reference to the dictionary.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
func withUnsafeUnderlyingDictionary(_ closure: (xpc_object_t) throws -> ReturnType) rethrows -> ReturnType
```

## Parameters 

`closure`  

A closure that takes an xpc_object_t parameter. If `closure` has a return value, that value is also used as the return value for the withUnsafeUnderlyingDictionary(body:) function.

## Return Value

The return value, if any, of the closure.

## Discussion

Warning

It’s possible for `closure` to perform operations on the dictionary that cause the receiving dictionary to no longer wrap the underlying dictionary.

## See Also

### Accessing keys and values

var keys: [String]

A collection containing just the keys of the dictionary.

var values: [xpc_object_t]

A collection containing just the values of the dictionary.

subscript(String) -> XPCDictionary?

Reads and writes the value associated with the given key as an XPC dictionary.

subscript(String) -> String?

Reads and writes the value associated with the given key as a string.

subscript(String) -> Bool?

Reads and writes the value associated with the given key as a Boolean value.

subscript(String) -> xpc_object_t?

Reads and writes the value associated with the given key as an XPC object.

subscript&lt;T>(String) -> T?

Reads and writes the value associated with the given key as a floating point value.

subscript&lt;T>(String) -> T?

Reads and writes the value associated with the given key as an unsigned integer value.

subscript&lt;T>(String) -> T?

Reads and writes the value associated with the given key as a signed integer value.

subscript(String, as _: XPCDictionary.Type) -> XPCDictionary?

Reads the value associated with the given key as an XPC dictionary.

subscript(String, as _: String.Type) -> String?

Reads and writes the value associated with the given key as a string.

subscript(String, as _: Bool.Type) -> Bool?

Reads and writes the value associated with the given key as a Boolean value.

subscript(String, as _: any OS_xpc_object.Type) -> xpc_object_t?

Reads and writes the value associated with the given key as an XPC object.

subscript(String, as _: xpc_type_t) -> xpc_object_t?

Reads and writes the value associated with the given key as an XPC object.

subscript&lt;T>(String, as _: T.Type) -> T?

Reads and writes the value associated with the given key as a floating point value.

