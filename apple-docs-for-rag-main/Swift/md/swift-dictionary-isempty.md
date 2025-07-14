

- Swift
- Dictionary
-  isEmpty 

Instance Property

# isEmpty

A Boolean value that indicates whether the dictionary is empty.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isEmpty: Bool { get }
```

Available when `Key` conforms to `Hashable`.

## Discussion

Dictionaries are empty when created with an initializer or an empty dictionary literal.

```
var frequencies: [String: Int] = [:]
print(frequencies.isEmpty)
// Prints "true"
```

## See Also

### Inspecting a Dictionary

var count: Int

The number of key-value pairs in the dictionary.

var capacity: Int

The total number of key-value pairs that the dictionary can contain without allocating new storage.

