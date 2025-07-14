

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
-  vCard Deprecated

Type Property

# vCard

VCard data.

macOS 10.0–10.14Deprecated

``` source
static let vCard: NSPasteboard.PasteboardType
```

## Discussion

In macOS 10.6 and later, use `(NSString *)kUTTypeVCard` instead.

## See Also

### Deprecated

static let filePromise: NSPasteboard.PasteboardType

Promised files.

Deprecated

static let inkText: NSPasteboard.PasteboardType

Ink text data.

Deprecated

static let postScript: NSPasteboard.PasteboardType

Encapsulated PostScript (EPS) code.

Deprecated

var representedPathExtension: String?

A file type based on the passed pasteboard type.

Deprecated

static func fileContentsType(forPathExtension: String) -> NSPasteboard.PasteboardType!

Returns a pasteboard type based on the passed file type.

Deprecated

static func fileNameType(forPathExtension: String) -> NSPasteboard.PasteboardType!

Returns a pasteboard type based on the passed file type.

Deprecated

static func representedPathExtensions(from: [NSPasteboard.PasteboardType]) -> [String]?

Returns an array of file types based on the passed pasteboard types.

Deprecated

