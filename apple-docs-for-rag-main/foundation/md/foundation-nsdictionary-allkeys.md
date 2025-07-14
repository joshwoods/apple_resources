

- Foundation
- NSDictionary
-  allKeys 

Instance Property

# allKeys

A new array containing the dictionary’s keys, or an empty array if the dictionary has no entries.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allKeys: [Any] { get }
```

## Discussion

The order of the elements in the array is not defined.

## See Also

### Accessing Keys and Values

func allKeys(for: Any) -> [Any]

Returns a new array containing the keys corresponding to all occurrences of a given object in the dictionary.

var allValues: [Any]

A new array containing the dictionary’s values, or an empty array if the dictionary has no entries.

func value(forKey: String) -> Any?

Returns the value associated with a given key.

func objects(forKeys: [Any], notFoundMarker: Any) -> [Any]

Returns as a static array the set of objects from the dictionary that corresponds to the specified keys.

func object(forKey: Any) -> Any?

Returns the value associated with a given key.

subscript(any NSCopying) -> Any?

Returns the value associated with a given key.

subscript(Any) -> Any?

Accesses the value associated with a given key.

