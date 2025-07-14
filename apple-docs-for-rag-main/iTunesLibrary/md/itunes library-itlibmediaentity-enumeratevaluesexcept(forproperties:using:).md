

- iTunes Library
- ITLibMediaEntity
-  enumerateValuesExcept(forProperties:using:) 

Instance Method

# enumerateValuesExcept(forProperties:using:)

Executes a provided block with the fetched values for all properties in the entity except for the provided set.

Mac Catalyst 14.0+macOS 10.13+

``` source
func enumerateValuesExcept(
    forProperties properties: Set?,
    using block: @escaping (String, Any, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`properties`  

A set of keys for the properties to enumerate, or `nil` to enumerate all properties. Takes Media Item Properties and Playlist Properties from ITLibMediaItem.

`block`  

A block object that executes for each property in the properties set.

## Discussion

Use this method to get property values in a batch fashion. In some cases, enumerating over a set of property keys can be more efficient than fetching each individual property with value(forProperty:).

## See Also

### Getting Media Item Properties

func enumerateValues(forProperties: Set&lt;String>?, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for the item properties.

func value(forProperty: String) -> Any?

Gets the value for a specified media property key.

