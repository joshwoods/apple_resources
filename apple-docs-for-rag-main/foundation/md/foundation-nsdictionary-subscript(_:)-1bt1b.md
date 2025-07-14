

- Foundation
- NSDictionary
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the value associated with a given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@objc
dynamic subscript(key: Any) -> Any? { get }
```

## Parameters 

`key`  

The key whose value you want to retrieve.

## Discussion

The returned value is `nil` if `key` does not exist in the dictionary.

The listing below creates a new dictionary. It prints the value of a key found in the dictionary (`"Coral"`) and a key not found in the dictionary (`"Cerise"`).

```
var hues = NSDictionary(dictionary: ["Heliotrope": 296, "Coral": 16, "Aquamarine": 156])
print(hues["Coral"])
// Prints "Optional(16)"
print(hues["Cerise"])
// Prints "nil"

```

## See Also

### Accessing Keys and Values

var allKeys: [Any]

A new array containing the dictionary’s keys, or an empty array if the dictionary has no entries.

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

