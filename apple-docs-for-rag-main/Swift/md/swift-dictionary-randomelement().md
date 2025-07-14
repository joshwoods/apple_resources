

- Swift
- Dictionary
-  randomElement() 

Instance Method

# randomElement()

Returns a random element of the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func randomElement() -> Self.Element?
```

## Return Value

A random element from the collection. If the collection is empty, the method returns `nil`.

## Discussion

Call `randomElement()` to select a random element from an array or another collection. This example picks a name at random from an array:

```
let names = ["Zoey", "Chloe", "Amani", "Amaia"]
let randomName = names.randomElement()!
// randomName == "Amani"
```

This method is equivalent to calling `randomElement(using:)`, passing in the system’s default random generator.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

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

var values: Dictionary&lt;Key, Value>.Values

A collection containing just the values of the dictionary.

var first: Self.Element?

The first element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

