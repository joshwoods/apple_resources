

- AppKit
- NSWindow
-  titleVisibility 

Instance Property

# titleVisibility

A value that indicates the visibility of the window’s title and title bar buttons.

macOS 10.10+

``` source
@MainActor
var titleVisibility: NSWindow.TitleVisibility { get set }
```

## Discussion

By default, the value of this property is NSWindow.TitleVisibility.visible.

## See Also

### Managing Titles

var title: String

The string that appears in the title bar of the window or the path to the represented file.

var subtitle: String

A secondary line of text that appears in the title bar of the window.

func setTitleWithRepresentedFilename(String)

Sets a given path as the window’s title, formatting it as a file-system path, and records this path as the window’s associated file.

var representedFilename: String

The path to the file of the window’s represented file.

var representedURL: URL?

The URL of the file the window represents.

