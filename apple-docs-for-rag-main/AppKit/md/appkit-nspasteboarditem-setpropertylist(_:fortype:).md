

- AppKit
- NSPasteboardItem
-  setPropertyList(\_:forType:) 

Instance Method

# setPropertyList(\_:forType:)

Sets the value for a specified type as a property list.

macOS 10.6+

``` source
func setPropertyList(
    _ propertyList: Any,
    forType type: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`propertyList`  

A property list object containing the value for the representation specified by `type`.

`type`  

A uniform type identifier string.

## Return Value

true if the value was set successfully, otherwise false.

## See Also

### Setting values

func setData(Data, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a data object.

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a string.

