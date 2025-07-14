

- AppKit
- NSPasteboardItem
-  setData(\_:forType:) 

Instance Method

# setData(\_:forType:)

Sets the value for a specified type as a data object.

macOS 10.6+

``` source
func setData(
    _ data: Data,
    forType type: NSPasteboard.PasteboardType
) -> Bool
```

## Parameters 

`data`  

An `NSData` object containing the value for the representation specified by `type`.

`type`  

A uniform type identifier string.

## Return Value

true if the value was set successfully, otherwise false.

## See Also

### Setting values

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a string.

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the value for a specified type as a property list.

