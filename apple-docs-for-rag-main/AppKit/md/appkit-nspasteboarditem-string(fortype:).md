

- AppKit
- NSPasteboardItem
-  string(forType:) 

Instance Method

# string(forType:)

Returns the value for the specified type as a string.

macOS 10.6+

``` source
func string(forType type: NSPasteboard.PasteboardType) -> String?
```

## Parameters 

`type`  

A uniform type identifier string.

## Return Value

The value for the specified type as a string.

## See Also

### Getting values

func data(forType: NSPasteboard.PasteboardType) -> Data?

Returns the value for the specified type as a data object.

func propertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns the value for the specified type as a property list.

