

- AppKit
- NSPasteboard
- NSPasteboard.ReadingOptions
-  asData 

Type Property

# asData

An option to read data from the pasteboard as-is and return it as a data object.

macOS 10.6+

``` source
static var asData: NSPasteboard.ReadingOptions { get }
```

## Discussion

This is the default value. AppKit returns the data in an NSData object.

## See Also

### Options

static var asString: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and convert it to a string object.

static var asPropertyList: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and unserialize it as a property list.

static var asKeyedArchive: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and use it to initialize the object.

