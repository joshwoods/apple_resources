

- AppKit
- NSSplitViewItem
-  init(contentListWithViewController:) 

Initializer

# init(contentListWithViewController:)

Creates a split view item that represents a content list for the specified view controller.

macOS 10.11+

``` source
convenience init(contentListWithViewController viewController: NSViewController)
```

## Discussion

You use a content list to display information like the Mail app’s list of messages or the Notes app’s list of notes.

Content lists use standard system default values for these properties:

- minimumThickness, maximumThickness, and automaticMaximumThickness use the standard system defaults for content lists

- preferredThicknessFraction uses the standard fraction for content lists (`0.28` if an adjacent sidebar is visible, `0.33` if not)

## See Also

### Creating a Split View Item

convenience init(sidebarWithViewController: NSViewController)

Creates a split view item that represents a sidebar for the specified view controller.

convenience init(viewController: NSViewController)

Creates a split view item that represents the specified view controller.

convenience init(inspectorWithViewController: NSViewController)

