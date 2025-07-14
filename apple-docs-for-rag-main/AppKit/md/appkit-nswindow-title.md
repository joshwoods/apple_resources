

- AppKit
- NSWindow
-  title 

Instance Property

# title

The string that appears in the title bar of the window or the path to the represented file.

macOS

``` source
@MainActor
var title: String { get set }
```

## Discussion

If the title has been set using setTitleWithRepresentedFilename(_:), this property contains the file’s path. Setting this property also sets the title of the window’s miniaturized window.

## See Also

### Related Documentation

var miniwindowTitle: String!

The title displayed in the window’s minimized window.

### Managing Titles

var subtitle: String

A secondary line of text that appears in the title bar of the window.

var titleVisibility: NSWindow.TitleVisibility

A value that indicates the visibility of the window’s title and title bar buttons.

func setTitleWithRepresentedFilename(String)

Sets a given path as the window’s title, formatting it as a file-system path, and records this path as the window’s associated file.

var representedFilename: String

The path to the file of the window’s represented file.

var representedURL: URL?

The URL of the file the window represents.

