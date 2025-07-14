

- Swift
- Dictionary
-  values 

Instance Property

# values

A collection containing just the values of the dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+Swift 4.0+

``` source
var values: Dictionary.Values { get set }
```

Available when `Key` conforms to `Hashable`.

## Discussion

When iterated over, values appear in this collection in the same order as they occur in the dictionary’s key-value pairs.

```
let countryCodes = ["BR": "Brazil", "GH": "Ghana", "JP": "Japan"]
print(countryCodes)
// Prints "["BR": "Brazil", "JP": "Japan", "GH": "Ghana"]"

for v in countryCodes.values {
    print(v)
}
// Prints "Brazil"
// Prints "Japan"
// Prints "Ghana"
```

## See Also

### Accessing Keys and Values

subscript(Key) -> Value?

Accesses the value associated with the given key for reading and writing.

subscript(Key, default _: @autoclosure () -> Value) -> Value

Accesses the value with the given key, falling back to the given default value if the key isn’t found.

func index(forKey: Key) -> Dictionary&lt;Key, Value>.Index?

Returns the index for the given key.

subscript(Dictionary&lt;Key, Value>.Index) -> Dictionary&lt;Key, Value>.Element

Accesses the key-value pair at the specified position.

var keys: Dictionary&lt;Key, Value>.Keys

A collection containing just the keys of the dictionary.

var first: Self.Element?

The first element of the collection.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

