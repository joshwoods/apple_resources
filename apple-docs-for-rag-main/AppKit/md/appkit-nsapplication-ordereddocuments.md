

- AppKit
- NSApplication
-  orderedDocuments 

Instance Property

# orderedDocuments

An array of document objects arranged according to the front-to-back ordering of their associated windows.

macOS

``` source
@MainActor
var orderedDocuments: [NSDocument] { get }
```

## See Also

### Scripting Your App

var orderedWindows: [NSWindow]

An array of window objects arranged according to their front-to-back ordering on the screen.

