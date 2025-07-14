

- XPC
- XPCDictionary
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Reads and writes the value associated with the given key as an XPC dictionary.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
subscript(key: String) -> XPCDictionary? { get set }
```

## Parameters 

`key`  

The key the look up in the dictionary.

## Return Value

The value associated with key in the dictionary; otherwise, Nil.

## See Also

### Accessing keys and values

var keys: [String]

A collection containing just the keys of the dictionary.

var values: [xpc_object_t]

A collection containing just the values of the dictionary.

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

subscript&lt;T>(String, as _: T.Type) -> T?

Reads and writes the value associated with the given key as an integer value.

