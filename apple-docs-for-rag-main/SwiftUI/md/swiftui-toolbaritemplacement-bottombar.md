

- SwiftUI
- ToolbarItemPlacement
-  bottomBar 

Type Property

# bottomBar

Places the item in the bottom toolbar.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 18.0+visionOS 1.0+watchOS 10.0+

``` source
static let bottomBar: ToolbarItemPlacement
```

## Discussion

On tvOS, this applies only within the sidebar of a NavigationSplitView. It has no effect if used elsewhere.

## See Also

### Getting explicit placement

static var topBarLeading: ToolbarItemPlacement

Places the item in the leading edge of the top bar.

static var topBarTrailing: ToolbarItemPlacement

Places the item in the trailing edge of the top bar.

static let bottomOrnament: ToolbarItemPlacement

Places the item in an ornament under the window.

static let keyboard: ToolbarItemPlacement

The item is placed in the keyboard section.

static func accessoryBar&lt;ID>(id: ID) -> ToolbarItemPlacement

Creates a unique accessory bar placement.

