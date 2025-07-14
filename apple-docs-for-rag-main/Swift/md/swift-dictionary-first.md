

- Swift
- Dictionary
-  first 

Instance Property

# first

The first element of the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var first: Self.Element? { get }
```

## Discussion

If the collection is empty, the value of this property is `nil`.

```
let numbers = [10, 20, 30, 40, 50]
if let firstNumber = numbers.first {
    print(firstNumber)
}
// Prints "10"
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

var values: Dictionary&lt;Key, Value>.Values

A collection containing just the values of the dictionary.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

