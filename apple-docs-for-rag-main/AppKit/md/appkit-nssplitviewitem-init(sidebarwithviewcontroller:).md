

- AppKit
- NSSplitViewItem
-  init(sidebarWithViewController:) 

Initializer

# init(sidebarWithViewController:)

Creates a split view item that represents a sidebar for the specified view controller.

macOS 10.11+

``` source
convenience init(sidebarWithViewController viewController: NSViewController)
```

## Discussion

Sidebar items take advantage of the standard system appearance and behavior for sidebars, including:

- The translucent material background

- The ability to collapse and expand on split view size changes

- The ability to overlay at small split view sizes in full-screen mode

Additionally, sidebars use standard system default values for these properties:

- canCollapse and isSpringLoaded are true

- minimumThickness and maximumThickness use the standard minimum and maximum sidebar size

- preferredThicknessFraction uses the standard fraction for sidebars (`0.15`)

## See Also

### Creating a Split View Item

convenience init(contentListWithViewController: NSViewController)

Creates a split view item that represents a content list for the specified view controller.

convenience init(viewController: NSViewController)

Creates a split view item that represents the specified view controller.

convenience init(inspectorWithViewController: NSViewController)

