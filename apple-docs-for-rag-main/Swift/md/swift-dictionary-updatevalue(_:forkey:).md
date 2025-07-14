

- Swift
- Dictionary
-  updateValue(\_:forKey:) 

Instance Method

# updateValue(\_:forKey:)

Updates the value stored in the dictionary for the given key, or adds a new key-value pair if the key does not exist.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func updateValue(
    _ value: Value,
    forKey key: Key
) -> Value?
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`value`  

The new value to add to the dictionary.

`key`  

The key to associate with `value`. If `key` already exists in the dictionary, `value` replaces the existing associated value. If `key` isn’t already a key of the dictionary, the `(key, value)` pair is added.

## Return Value

The value that was replaced, or `nil` if a new key-value pair was added.

## Discussion

Use this method instead of key-based subscripting when you need to know whether the new value supplants the value of an existing key. If the value of an existing key is updated, `updateValue(_:forKey:)` returns the original value.

```
var hues = ["Heliotrope": 296, "Coral": 16, "Aquamarine": 156]

if let oldValue = hues.updateValue(18, forKey: "Coral") {
    print("The old value of \(oldValue) was replaced with a new one.")
}
// Prints "The old value of 16 was replaced with a new one."
```

If the given key is not present in the dictionary, this method adds the key-value pair and returns `nil`.

```
if let oldValue = hues.updateValue(330, forKey: "Cerise") {
    print("The old value of \(oldValue) was replaced with a new one.")
} else {
    print("No value was found in the dictionary for that key.")
}
// Prints "No value was found in the dictionary for that key."
```

## See Also

### Adding Keys and Values

func merge([Key : Value], uniquingKeysWith: (Value, Value) throws -> Value) rethrows

Merges the given dictionary into this dictionary, using a combining closure to determine the value for any duplicate keys.

func merge&lt;S>(S, uniquingKeysWith: (Value, Value) throws -> Value) rethrows

Merges the key-value pairs in the given sequence into the dictionary, using a combining closure to determine the value for any duplicate keys.

func merging([Key : Value], uniquingKeysWith: (Value, Value) throws -> Value) rethrows -> [Key : Value]

Creates a dictionary by merging the given dictionary into this dictionary, using a combining closure to determine the value for duplicate keys.

func merging&lt;S>(S, uniquingKeysWith: (Value, Value) throws -> Value) rethrows -> [Key : Value]

Creates a dictionary by merging key-value pairs in a sequence into the dictionary, using a combining closure to determine the value for duplicate keys.

func reserveCapacity(Int)

Reserves enough space to store the specified number of key-value pairs.

