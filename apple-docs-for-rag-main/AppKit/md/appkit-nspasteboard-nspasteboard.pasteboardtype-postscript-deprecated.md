

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
-  postScript Deprecated

Type Property

# postScript

Encapsulated PostScript (EPS) code.

macOS 10.0–10.14Deprecated

``` source
static let postScript: NSPasteboard.PasteboardType
```

## Discussion

In macOS 10.6 and later, use `@"com.adobe.encapsulated-postscript"` instead.

## See Also

### Deprecated

static let filePromise: NSPasteboard.PasteboardType

Promised files.

Deprecated

static let inkText: NSPasteboard.PasteboardType

Ink text data.

Deprecated

static let vCard: NSPasteboard.PasteboardType

VCard data.

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

