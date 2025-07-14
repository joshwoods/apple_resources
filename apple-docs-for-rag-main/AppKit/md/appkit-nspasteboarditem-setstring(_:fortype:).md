

- AppKit
- NSPasteboardItem
-  setString(\_:forType:) 

Instance Method

# setString(\_:forType:)

Sets the value for a specified type as a string.

macOS 10.6+

``` source
func setString(
    _ string: String,
    forType type: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`string`  

A string for the representation specified by `type`.

`type`  

A uniform type identifier string.

## Return Value

true if the value was set successfully, otherwise false.

## See Also

### Setting values

func setData(Data, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a data object.

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a property list.

