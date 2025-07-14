

- AppKit
- NSPasteboard
- NSPasteboard.ReadingOptions
-  asKeyedArchive 

Type Property

# asKeyedArchive

An option to read data from the pasteboard and use it to initialize the object.

macOS 10.6+

``` source
static var asKeyedArchive: NSPasteboard.ReadingOptions { get }
```

## Discussion

AppKit initializes the object using its init(coder:) method.

## See Also

### Options

static var asData: NSPasteboard.ReadingOptions

An option to read data from the pasteboard as-is and return it as a data object.

static var asString: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and convert it to a string object.

static var asPropertyList: NSPasteboard.ReadingOptions

An option to read data from the pasteboard and unserialize it as a property list.

