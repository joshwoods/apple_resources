

- AppKit
- NSPasteboardItem
-  data(forType:) 

Instance Method

# data(forType:)

Returns the value for the specified type as a data object.

macOS 10.6+

``` source
func data(forType type: NSPasteboard.PasteboardType) -> Data?
```

## Parameters 

`type`  

A uniform type identifier string.

## Return Value

The value for the specified type as an `NSData` object.

## See Also

### Getting values

func string(forType: NSPasteboard.PasteboardType) -> String?

Returns the value for the specified type as a string.

func propertyList(forType: NSPasteboard.PasteboardType) -> Any?

Returns the value for the specified type as a property list.

