

- Swift
- Dictionary
-  removeValue(forKey:) 

Instance Method

# removeValue(forKey:)

Removes the given key and its associated value from the dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func removeValue(forKey key: Key) -> Value?
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`key`  

The key to remove along with its associated value.

## Return Value

The value that was removed, or `nil` if the key was not present in the dictionary.

## Discussion

If the key is found in the dictionary, this method returns the key’s associated value. On removal, this method invalidates all indices with respect to the dictionary.

```
var hues = ["Heliotrope": 296, "Coral": 16, "Aquamarine": 156]
if let value = hues.removeValue(forKey: "Coral") {
    print("The value \(value) was removed.")
}
// Prints "The value 16 was removed."
```

If the key isn’t found in the dictionary, `removeValue(forKey:)` returns `nil`.

```
if let value = hues.removeValue(forKey: "Cerise") {
    print("The value \(value) was removed.")
} else {
    print("No value found for that key.")
}
// Prints "No value found for that key."
```

Complexity

O(*n*), where *n* is the number of key-value pairs in the dictionary.

## See Also

### Removing Keys and Values

func filter((Dictionary&lt;Key, Value>.Element) throws -> Bool) rethrows -> [Key : Value]

Returns a new dictionary containing the key-value pairs of the dictionary that satisfy the given predicate.

func remove(at: Dictionary&lt;Key, Value>.Index) -> Dictionary&lt;Key, Value>.Element

Removes and returns the key-value pair at the specified index.

func removeAll(keepingCapacity: Bool)

Removes all key-value pairs from the dictionary.

