

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
-  html 

Type Property

# html

Type for HTML content.

macOS 10.6+

``` source
static let html: NSPasteboard.PasteboardType
```

## Discussion

An `NSTextView` object can read HTML data, but not write it.

In macOS 10.6 and later, use html instead.

## See Also

### Pasteboard Types

static let URL: NSPasteboard.PasteboardType

URL data for one file or resource.

static let collaborationMetadata: NSPasteboard.PasteboardType

An object you use for conveying data during a collaboration.

static let color: NSPasteboard.PasteboardType

Color data.

static let fileContents: NSPasteboard.PasteboardType

A representation of a file’s contents.

static let fileURL: NSPasteboard.PasteboardType

A file URL.

static let findPanelSearchOptions: NSPasteboard.PasteboardType

Type for the find panel metadata property list.

static let font: NSPasteboard.PasteboardType

Font and character information.

static let multipleTextSelection: NSPasteboard.PasteboardType

Multiple text selection.

static let pdf: NSPasteboard.PasteboardType

PDF data.

static let png: NSPasteboard.PasteboardType

PNG image data.

static let rtf: NSPasteboard.PasteboardType

Rich Text Format (RTF) data.

static let rtfd: NSPasteboard.PasteboardType

RTFD formatted file contents.

static let ruler: NSPasteboard.PasteboardType

Paragraph formatting information.

static let sound: NSPasteboard.PasteboardType

Sound data.

static let string: NSPasteboard.PasteboardType

String data.

