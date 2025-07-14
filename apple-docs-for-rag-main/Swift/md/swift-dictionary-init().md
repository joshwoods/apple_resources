

- Swift
- Dictionary
-  init() 

Initializer

# init()

Creates an empty dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

## See Also

### Creating a Dictionary

init(minimumCapacity: Int)

Creates an empty dictionary with preallocated space for at least the specified number of elements.

init&lt;S>(uniqueKeysWithValues: S)

Creates a new dictionary from the key-value pairs in the given sequence.

init&lt;S>(S, uniquingKeysWith: (Value, Value) throws -> Value) rethrows

Creates a new dictionary from the key-value pairs in the given sequence, using a combining closure to determine the value for any duplicate keys.

init&lt;S>(grouping: S, by: (S.Element) throws -> Key) rethrows

Creates a new dictionary whose keys are the groupings returned by the given closure and whose values are arrays of the elements that returned each key.

