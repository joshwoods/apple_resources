

- Swift
- Dictionary
-  remove(at:) 

Instance Method

# remove(at:)

Removes and returns the key-value pair at the specified index.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func remove(at index: Dictionary.Index) -> Dictionary.Element
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`index`  

The position of the key-value pair to remove. `index` must be a valid index of the dictionary, and must not equal the dictionary’s end index.

## Return Value

The key-value pair that correspond to `index`.

## Discussion

Calling this method invalidates any existing indices for use with this dictionary.

Complexity

O(*n*), where *n* is the number of key-value pairs in the dictionary.

## See Also

### Removing Keys and Values

func filter((Dictionary&lt;Key, Value>.Element) throws -> Bool) rethrows -> [Key : Value]

Returns a new dictionary containing the key-value pairs of the dictionary that satisfy the given predicate.

func removeValue(forKey: Key) -> Value?

Removes the given key and its associated value from the dictionary.

func removeAll(keepingCapacity: Bool)

Removes all key-value pairs from the dictionary.

