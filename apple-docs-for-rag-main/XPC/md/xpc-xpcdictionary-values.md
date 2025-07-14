

- XPC
- XPCDictionary
-  values 

Instance Property

# values

A collection containing just the values of the dictionary.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
var values: [xpc_object_t] { get }
```

## Discussion

A collection containing just the values of the dictionary. When iterated over, values appear in this collection in the same order as they occur in the dictionary’s key-value pairs.

Note

The complexity of this property is O(\*n\*) over the dictionary’s count.

## See Also

### Accessing keys and values

var keys: [String]

A collection containing just the keys of the dictionary.

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

subscript&lt;T>(String, as _: T.Type) -> T?

Reads and writes the value associated with the given key as an integer value.

