

- AppKit
- NSPasteboard
- NSPasteboard.Name
-  generalPboard Deprecated

Type Property

# generalPboard

The pasteboard used for ordinary cut, copy, and paste operations.

macOS 10.0–10.13Deprecated

``` source
static let generalPboard: NSPasteboard.Name
```

## Discussion

This pasteboard holds the contents of the last selection that’s been cut or copied.

## See Also

### Deprecated

static let dragPboard: NSPasteboard.Name

The pasteboard that stores data to be moved as the result of a drag operation.

Deprecated

static let findPboard: NSPasteboard.Name

The pasteboard that holds information about the current state of the active application’s find panel.

Deprecated

static let fontPboard: NSPasteboard.Name

The pasteboard that holds font and character information and supports Copy Font and Paste Font commands that may be implemented in a text editor.

Deprecated

static let rulerPboard: NSPasteboard.Name

The pasteboard that holds information about paragraph formats and supports the Copy Ruler and Paste Ruler commands implemented in a text editor.

Deprecated

