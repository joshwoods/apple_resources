

- AppKit
- NSWindow
-  representedFilename 

Instance Property

# representedFilename

The path to the file of the window’s represented file.

macOS

``` source
@MainActor
var representedFilename: String { get set }
```

## See Also

### Managing Titles

var title: String

The string that appears in the title bar of the window or the path to the represented file.

var subtitle: String

A secondary line of text that appears in the title bar of the window.

var titleVisibility: NSWindow.TitleVisibility

A value that indicates the visibility of the window’s title and title bar buttons.

func setTitleWithRepresentedFilename(String)

Sets a given path as the window’s title, formatting it as a file-system path, and records this path as the window’s associated file.

var representedURL: URL?

The URL of the file the window represents.

