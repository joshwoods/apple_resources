

- AppKit
- NSWindow
-  representedURL 

Instance Property

# representedURL

The URL of the file the window represents.

macOS 10.5+

``` source
@MainActor
var representedURL: URL? { get set }
```

## Discussion

When the URL specifies a path, the window shows an icon in its title bar, as described in the following table:

| File path                    | Document icon                |
|------------------------------|------------------------------|
| Empty                        | None                         |
| Specifies a nonexistent file | Generic                      |
| Specifies an existent file   | Specific for the file’s type |

You can customize the file icon in the title bar with the following code:

```
[[ standardWindowButton:NSWindowDocumentIconButton] setImage:]
```

When the URL identifies an existing file, the window’s title offers a pop-up menu showing the path components of the URL. (The user displays this menu by Command-clicking the title.) The behavior and contents of this menu can be controlled with window(_:shouldPopUpDocumentPathMenu:).

## See Also

### Related Documentation

func window(NSWindow, shouldDragDocumentWith: NSEvent, from: NSPoint, with: NSPasteboard) -> Bool

Asks the delegate whether a user can drag the document icon from the window’s title bar.

### Managing Titles

var title: String

The string that appears in the title bar of the window or the path to the represented file.

var subtitle: String

A secondary line of text that appears in the title bar of the window.

var titleVisibility: NSWindow.TitleVisibility

A value that indicates the visibility of the window’s title and title bar buttons.

func setTitleWithRepresentedFilename(String)

Sets a given path as the window’s title, formatting it as a file-system path, and records this path as the window’s associated file.

var representedFilename: String

The path to the file of the window’s represented file.

