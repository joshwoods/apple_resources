

- SwiftUI
- ToolbarPlacement
-  automatic 

Type Property

# automatic

The primary toolbar.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var automatic: ToolbarPlacement { get }
```

## Discussion

Depending on the context, this may refer to the navigation bar of an app on iOS, or watchOS, the tab bar of an app on tvOS, or the window toolbar / window titlebar of an app on macOS.

## See Also

### Getting placements

static func accessoryBar&lt;ID>(id: ID) -> ToolbarPlacement

Creates a unique accessory bar placement.

static var bottomBar: ToolbarPlacement

The bottom toolbar of an app.

static var bottomOrnament: ToolbarPlacement

The bottom ornament of an app.

static var navigationBar: ToolbarPlacement

The navigation bar of an app.

static var tabBar: ToolbarPlacement

The tab bar of an app.

static var windowToolbar: ToolbarPlacement

The placement for the containing window’s toolbar, sometimes referred to as the titlebar.

