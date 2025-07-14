

- Foundation
- NSDictionary
-  objects(forKeys:notFoundMarker:) 

Instance Method

# objects(forKeys:notFoundMarker:)

Returns as a static array the set of objects from the dictionary that corresponds to the specified keys.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func objects(
    forKeys keys: [Any],
    notFoundMarker marker: Any
) -> [Any]
```

## Parameters 

`keys`  

An `NSArray` containing the keys for which to return corresponding values.

`marker`  

The marker object to place in the corresponding element of the returned array if an object isn’t found in the dictionary to correspond to a given key.

## Discussion

The objects in the returned array and the `keys` array have a one-for-one correspondence, so that the nthe object in the returned array corresponds to the nthe key in `keys`.

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

func object(forKey: Any) -> Any?

Returns the value associated with a given key.

subscript(any NSCopying) -> Any?

Returns the value associated with a given key.

subscript(Any) -> Any?

Accesses the value associated with a given key.

