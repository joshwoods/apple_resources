

- Swift
- Dictionary
-  removeAll(keepingCapacity:) 

Instance Method

# removeAll(keepingCapacity:)

Removes all key-value pairs from the dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeAll(keepingCapacity keepCapacity: Bool = false)
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`keepCapacity`  

Whether the dictionary should keep its underlying buffer. If you pass `true`, the operation preserves the buffer capacity that the collection has, otherwise the underlying buffer is released. The default is `false`.

## Discussion

Calling this method invalidates all indices with respect to the dictionary.

Complexity

O(*n*), where *n* is the number of key-value pairs in the dictionary.

## See Also

### Removing Keys and Values

func filter((Dictionary&lt;Key, Value>.Element) throws -> Bool) rethrows -> [Key : Value]

Returns a new dictionary containing the key-value pairs of the dictionary that satisfy the given predicate.

func removeValue(forKey: Key) -> Value?

Removes the given key and its associated value from the dictionary.

func remove(at: Dictionary&lt;Key, Value>.Index) -> Dictionary&lt;Key, Value>.Element

Removes and returns the key-value pair at the specified index.

