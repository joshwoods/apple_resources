

- AppKit
- NSWindow
-  subtitle 

Instance Property

# subtitle

A secondary line of text that appears in the title bar of the window.

macOS 11.0+

``` source
@MainActor
var subtitle: String { get set }
```

## Discussion

When this property is an empty string, the system removes the subtitle from the window layout.

## See Also

### Managing Titles

var title: String

The string that appears in the title bar of the window or the path to the represented file.

var titleVisibility: NSWindow.TitleVisibility

A value that indicates the visibility of the window’s title and title bar buttons.

func setTitleWithRepresentedFilename(String)

Sets a given path as the window’s title, formatting it as a file-system path, and records this path as the window’s associated file.

var representedFilename: String

The path to the file of the window’s represented file.

var representedURL: URL?

The URL of the file the window represents.

