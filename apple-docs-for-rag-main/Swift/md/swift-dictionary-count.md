

- Swift
- Dictionary
-  count 

Instance Property

# count

The number of key-value pairs in the dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var count: Int { get }
```

Available when `Key` conforms to `Hashable`.

## Discussion

Complexity

O(1).

## See Also

### Inspecting a Dictionary

var isEmpty: Bool

A Boolean value that indicates whether the dictionary is empty.

var capacity: Int

The total number of key-value pairs that the dictionary can contain without allocating new storage.

