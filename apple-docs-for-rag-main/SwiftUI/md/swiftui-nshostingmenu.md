

- SwiftUI
-  NSHostingMenu 

Class

# NSHostingMenu

An AppKit menu with menu items that are defined by a SwiftUI View.

macOS 14.4+

``` source
class NSHostingMenu where Content : View
```

## Overview

Because `NSHostingMenu` is an `NSMenu` subclass, you can integrate it into your existing AppKit view hierarchies that display menus. For example, you can set a hosting menu as an AppKit view’s context menu.

A hosting menu’s `items` property will be updated based on the content of the provided `rootView`, so direct mutations to the item array are not allowed, even if done using methods like `addItem` on the menu itself.

SwiftUI views hosted in the menu will be styled and behave identically to views in a Menu or `View/contextMenu`. Make sure to use a `Group` or a view with multiple subviews as your top level container instead of an `HStack` or other container that would attempt to place all of your actions in a single menu item.

Note

When used as the menu of an `NSPopUpButton`, make sure `NSPopUpButtonCell.usesItemFromMenu` is set to `false`. When using a hosting menu with macOS 14, do not change the value of the `delegate` property. (Setting the delegate is permitted on macOS 15 and newer.)

For example, the following code would set up the first part of the Finder’s context menu, both in the Action button in the toolbar and as a context menu:

```
struct FileOrFolderContextMenu: View {
    let url: URL
    var body: some View {
        Section {
            if url.hasDirectoryPath {
                Button("Open in New Tab") { ... }
            } else {
                Button("Open") { ... }
                Menu("Open With") { ... }
            }
        }
        Section {
            Button("Move to Trash") { ... }
        }
        Section {
            Button("Get Info") { ... }
            Button("Rename") { ... }
            if url.pathExtension != "zip" {
                Button("Compress “\(url.lastPathComponent)”") { ... }
            }
            // ...
        }
    }
}

// In the toolbar setup:
let popUpButton = NSPopUpButton(frame: .zero, pullsDown: true)
(popUpButton.cell as! NSPopUpButtonCell).usesItemFromMenu = false
popUpButton.menu = NSHostingMenu(rootView: Group {
    Button("New Folder") { ... }
    FileOrFolderContextMenu(url: selectedURL)
})

// In the column view:
List(directoryContents, selection: $selection) { entry in
    DirectoryEntryRow(entry: entry)
        .contextMenu {
            FileOrFolderContextMenu(url: entry.url)
        }
}
```

## Topics

### Initializers

init(rootView: Content)

Creates a hosting menu object that wraps the specified SwiftUI view.

### Instance Properties

var rootView: Content

The root view of the SwiftUI view hierarchy managed by this menu.

## Relationships

### Inherits From

- NSMenu

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAppearanceCustomization
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification

## See Also

### Displaying SwiftUI views in AppKit

Unifying your app’s animations

Create a consistent UI animation experience across SwiftUI, UIKit, and AppKit.

class NSHostingController

An AppKit view controller that hosts SwiftUI view hierarchy.

class NSHostingView

An AppKit view that hosts a SwiftUI view hierarchy.

struct NSHostingSizingOptions

Options for how hosting views and controllers reflect their content’s size into Auto Layout constraints.

struct NSHostingSceneBridgingOptions

Options for how hosting views and controllers manage aspects of the associated window.

