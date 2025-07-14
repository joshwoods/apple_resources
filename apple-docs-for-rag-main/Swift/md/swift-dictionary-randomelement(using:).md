

- Swift
- Dictionary
-  randomElement(using:) 

Instance Method

# randomElement(using:)

Returns a random element of the collection, using the given generator as a source for randomness.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func randomElement(using generator: inout T) -> Self.Element? where T : RandomNumberGenerator
```

## Parameters 

`generator`  

The random number generator to use when choosing a random element.

## Return Value

A random element from the collection. If the collection is empty, the method returns `nil`.

## Discussion

Call `randomElement(using:)` to select a random element from an array or another collection when you are using a custom random number generator. This example picks a name at random from an array:

```
let names = ["Zoey", "Chloe", "Amani", "Amaia"]
let randomName = names.randomElement(using: &myGenerator)!
// randomName == "Amani"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

Note

The algorithm used to select a random element may change in a future version of Swift. If you’re passing a generator that results in the same sequence of elements each time you run your program, that sequence may change when your program is compiled using a different version of Swift.

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

func randomElement() -> Self.Element?

Returns a random element of the collection.

