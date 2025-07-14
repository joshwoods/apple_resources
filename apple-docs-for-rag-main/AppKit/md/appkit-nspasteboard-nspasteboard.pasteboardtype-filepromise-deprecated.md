

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
-  filePromise Deprecated

Type Property

# filePromise

Promised files.

macOS 10.0–10.14Deprecated

``` source
static let filePromise: NSPasteboard.PasteboardType
```

## Discussion

In macOS 10.6 and later, use `(NSString *)kPasteboardTypeFileURLPromise` instead.

For information on promised files, see Dragging Files in Drag and Drop Programming Topics.

## See Also

### Deprecated

static let inkText: NSPasteboard.PasteboardType

Ink text data.

Deprecated

static let postScript: NSPasteboard.PasteboardType

Encapsulated PostScript (EPS) code.

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

