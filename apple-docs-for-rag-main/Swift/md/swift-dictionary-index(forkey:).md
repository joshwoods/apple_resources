

- Swift
- Dictionary
-  index(forKey:) 

Instance Method

# index(forKey:)

Returns the index for the given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(forKey key: Key) -> Dictionary.Index?
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`key`  

The key to find in the dictionary.

## Return Value

The index for `key` and its associated value if `key` is in the dictionary; otherwise, `nil`.

## Discussion

If the given key is found in the dictionary, this method returns an index into the dictionary that corresponds with the key-value pair.

```
let countryCodes = ["BR": "Brazil", "GH": "Ghana", "JP": "Japan"]
let index = countryCodes.index(forKey: "JP")

print("Country code for \(countryCodes[index!].value): '\(countryCodes[index!].key)'.")
// Prints "Country code for Japan: 'JP'."
```

## See Also

### Accessing Keys and Values

subscript(Key) -> Value?

Accesses the value associated with the given key for reading and writing.

subscript(Key, default _: @autoclosure () -> Value) -> Value

Accesses the value with the given key, falling back to the given default value if the key isn’t found.

subscript(Dictionary&lt;Key, Value>.Index) -> Dictionary&lt;Key, Value>.Element

Accesses the key-value pair at the specified position.

var keys: Dictionary&lt;Key, Value>.Keys

A collection containing just the keys of the dictionary.

var values: Dictionary&lt;Key, Value>.Values

A collection containing just the values of the dictionary.

var first: Self.Element?

The first element of the collection.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

