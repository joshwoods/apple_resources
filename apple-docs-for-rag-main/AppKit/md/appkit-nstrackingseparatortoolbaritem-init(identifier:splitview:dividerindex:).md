

- AppKit
- NSTrackingSeparatorToolbarItem
-  init(identifier:splitView:dividerIndex:) 

Initializer

# init(identifier:splitView:dividerIndex:)

Creates a new tracking separator toolbar item and configures it to align with the divider of the split view.

macOS 11.0+

``` source
@MainActor
convenience init(
    identifier: NSToolbarItem.Identifier,
    splitView: NSSplitView,
    dividerIndex: Int
)
```

## Parameters 

`identifier`  

The identifier of the toolbar item.

`splitView`  

The split view to align with the tracking separator.

`dividerIndex`  

The index of the divider in the split view.

