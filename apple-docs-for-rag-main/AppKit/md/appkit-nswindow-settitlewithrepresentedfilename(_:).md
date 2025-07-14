

- AppKit
- NSWindow
-  setTitleWithRepresentedFilename(\_:) 

Instance Method

# setTitleWithRepresentedFilename(\_:)

Sets a given path as the window’s title, formatting it as a file-system path, and records this path as the window’s associated file.

macOS

``` source
@MainActor
func setTitleWithRepresentedFilename(_ filename: String)
```

## Parameters 

`filename`  

The file path to set as the window’s title.

## Discussion

The windows’ title bar displays the filename, not the file’s path.

## See Also

### Related Documentation

var miniwindowTitle: String!

The title displayed in the window’s minimized window.

### Managing Titles

var title: String

The string that appears in the title bar of the window or the path to the represented file.

var subtitle: String

A secondary line of text that appears in the title bar of the window.

var titleVisibility: NSWindow.TitleVisibility

A value that indicates the visibility of the window’s title and title bar buttons.

var representedFilename: String

The path to the file of the window’s represented file.

var representedURL: URL?

The URL of the file the window represents.

