

- AppKit
- NSPasteboard
- NSPasteboard.ReadingOptions
-  asString 

Type Property

# asString

An option to read data from the pasteboard and convert it to a string object.

macOS 10.6+

``` source
static var asString: NSPasteboard.ReadingOptions { get }
```

## Discussion

AppKit puts the data in an NSString object.

## See Also

### Options

static var asData: NSPasteboard.ReadingOptions

An option to read data from the pasteboard as-is and return it as a data object.

static var asPropertyList: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and unserialize it as a property list.

static var asKeyedArchive: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and use it to initialize the object.

