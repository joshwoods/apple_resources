

- AppKit
- NSPasteboard
- NSPasteboard.ReadingOptions
-  asPropertyList 

Type Property

# asPropertyList

An option to read data from the pasteboard and unserialize it as a property list.

macOS 10.6+

``` source
static var asPropertyList: NSPasteboard.ReadingOptions { get }
```

## See Also

### Options

static var asData: NSPasteboard.ReadingOptions

An option to read data from the pasteboard as-is and return it as a data object.

static var asString: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and convert it to a string object.

static var asKeyedArchive: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and use it to initialize the object.

