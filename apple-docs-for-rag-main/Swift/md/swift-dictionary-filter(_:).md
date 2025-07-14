

- Swift
- Dictionary
-  filter(\_:) 

Instance Method

# filter(\_:)

Returns a new dictionary containing the key-value pairs of the dictionary that satisfy the given predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+Swift 4.0+

``` source
func filter(_ isIncluded: (Dictionary.Element) throws -> Bool) rethrows -> [Key : Value]
```

Available when `Key` conforms to `Hashable`.

## Parameters 

`isIncluded`  

A closure that takes a key-value pair as its argument and returns a Boolean value indicating whether the pair should be included in the returned dictionary.

## Return Value

A dictionary of the key-value pairs that `isIncluded` allows.

## See Also

### Removing Keys and Values

func removeValue(forKey: Key) -> Value?

Removes the given key and its associated value from the dictionary.

func remove(at: Dictionary&lt;Key, Value>.Index) -> Dictionary&lt;Key, Value>.Element

Removes and returns the key-value pair at the specified index.

func removeAll(keepingCapacity: Bool)

Removes all key-value pairs from the dictionary.

