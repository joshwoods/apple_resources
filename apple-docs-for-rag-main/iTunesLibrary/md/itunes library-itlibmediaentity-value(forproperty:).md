

- iTunes Library
- ITLibMediaEntity
-  value(forProperty:) 

Instance Method

# value(forProperty:)

Gets the value for a specified media property key.

Mac Catalyst 14.0+macOS 10.13+

``` source
func value(forProperty property: String) -> Any?
```

## Parameters 

`property`  

The media property to retrieve the value from. Takes Media Item Properties and Playlist Properties from ITLibMediaItem.

## Return Value

The value of the specified media property key.

## See Also

### Getting Media Item Properties

func enumerateValues(forProperties: Set&lt;String>?, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for the item properties.

func enumerateValuesExcept(forProperties: Set&lt;String>?, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for all properties in the entity except for the provided set.

