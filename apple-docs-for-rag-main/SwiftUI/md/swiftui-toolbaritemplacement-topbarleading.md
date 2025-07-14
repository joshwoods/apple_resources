

- SwiftUI
- ToolbarItemPlacement
-  topBarLeading 

Type Property

# topBarLeading

Places the item in the leading edge of the top bar.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
@backDeployed(before: iOS 17.0, tvOS 17.0)
static var topBarLeading: ToolbarItemPlacement { get }
```

## Discussion

On watchOS, iOS, and tvOS, the top bar is the navigation bar.

## See Also

### Getting explicit placement

static var topBarTrailing: ToolbarItemPlacement

Places the item in the trailing edge of the top bar.

static let bottomBar: ToolbarItemPlacement

Places the item in the bottom toolbar.

static let bottomOrnament: ToolbarItemPlacement

Places the item in an ornament under the window.

static let keyboard: ToolbarItemPlacement

The item is placed in the keyboard section.

static func accessoryBar&lt;ID>(id: ID) -> ToolbarItemPlacement

Creates a unique accessory bar placement.

