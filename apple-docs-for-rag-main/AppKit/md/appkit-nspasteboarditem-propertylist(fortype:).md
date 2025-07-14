

- AppKit
- NSPasteboardItem
-  propertyList(forType:) 

Instance Method

# propertyList(forType:)

Returns the value for the specified type as a property list.

macOS 10.6+

``` source
func propertyList(forType type: NSPasteboard.PasteboardType) -> Any?
```

## Parameters 

`type`  

A uniform type identifier string.

## Return Value

The value for the specified type as a property list.

## See Also

### Getting values

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the value for the specified type as a data object.

func string(forType: NSPasteboard.PasteboardType) -> String?

Returns the value for the specified type as a string.

