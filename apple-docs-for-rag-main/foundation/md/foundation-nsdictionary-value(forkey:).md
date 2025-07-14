

- Foundation
- NSDictionary
-  value(forKey:) 

Instance Method

# value(forKey:)

Returns the value associated with a given key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(forKey key: String) -> Any?
```

## Parameters 

`key`  

The key for which to return the corresponding value. Note that when using key-value coding, the key must be a string (see Accessing Object Properties).

## Return Value

The value associated with `key`.

## Discussion

If `key` does not start with “`@`”, invokes object(forKey:). If `key` does start with “`@`”, strips the “@” and invokes `[super valueForKey:]` with the rest of the key.

## See Also

### Related Documentation

func setValue(Any?, forKey: String)

Adds a given key-value pair to the dictionary.

### Accessing Keys and Values

var allKeys: [Any]

A new array containing the dictionary’s keys, or an empty array if the dictionary has no entries.

func allKeys(for: Any) -> [Any]

Returns a new array containing the keys corresponding to all occurrences of a given object in the dictionary.

var allValues: [Any]

A new array containing the dictionary’s values, or an empty array if the dictionary has no entries.

func objects(forKeys: [Any], notFoundMarker: Any) -> [Any]

Returns as a static array the set of objects from the dictionary that corresponds to the specified keys.

func object(forKey: Any) -> Any?

Returns the value associated with a given key.

subscript(any NSCopying) -> Any?

Returns the value associated with a given key.

subscript(Any) -> Any?

Accesses the value associated with a given key.

