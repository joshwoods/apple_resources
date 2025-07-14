

- Foundation
- NSDictionary
-  object(forKey:) 

Instance Method

# object(forKey:)

Returns the value associated with a given key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func object(forKey aKey: Any) -> Any?
```

## Parameters 

`aKey`  

The key for which to return the corresponding value.

## Return Value

The value associated with `aKey`, or `nil` if no value is associated with `aKey`.

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

subscript(any NSCopying) -> Any?

Returns the value associated with a given key.

subscript(Any) -> Any?

Accesses the value associated with a given key.

