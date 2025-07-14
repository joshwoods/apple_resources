

- Swift
- Dictionary
-  merge(\_:uniquingKeysWith:) 

Instance Method

# merge(\_:uniquingKeysWith:)

Merges the key-value pairs in the given sequence into the dictionary, using a combining closure to determine the value for any duplicate keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func merge(
    _ other: S,
    uniquingKeysWith combine: (Value, Value) throws -> Value
) rethrows where S : Sequence, S.Element == (Key, Value)
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`other`  

A sequence of key-value pairs.

`combine`  

A closure that takes the current and new values for any duplicate keys. The closure returns the desired value for the final dictionary.

## Discussion

Use the `combine` closure to select a value to use in the updated dictionary, or to combine existing and new values. As the key-value pairs are merged with the dictionary, the `combine` closure is called with the current and new values for any duplicate keys that are encountered.

This example shows how to choose the current or new values for any duplicate keys:

```
var dictionary = ["a": 1, "b": 2]

// Keeping existing value for key "a":
dictionary.merge(zip(["a", "c"], [3, 4])) { (current, _) in current }
// ["b": 2, "a": 1, "c": 4]

// Taking the new value for key "a":
dictionary.merge(zip(["a", "d"], [5, 6])) { (_, new) in new }
// ["b": 2, "a": 5, "c": 4, "d": 6]
```

## See Also

### Adding Keys and Values

func updateValue(Value, forKey: Key) -> Value?

Updates the value stored in the dictionary for the given key, or adds a new key-value pair if the key does not exist.

func merge([Key : Value], uniquingKeysWith: (Value, Value) throws -> Value) rethrows

Merges the given dictionary into this dictionary, using a combining closure to determine the value for any duplicate keys.

func merging([Key : Value], uniquingKeysWith: (Value, Value) throws -> Value) rethrows -> [Key : Value]

Creates a dictionary by merging the given dictionary into this dictionary, using a combining closure to determine the value for duplicate keys.

func merging&lt;S>(S, uniquingKeysWith: (Value, Value) throws -> Value) rethrows -> [Key : Value]

Creates a dictionary by merging key-value pairs in a sequence into the dictionary, using a combining closure to determine the value for duplicate keys.

func reserveCapacity(Int)

Reserves enough space to store the specified number of key-value pairs.

