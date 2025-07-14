

- SwiftUI
- ToolbarPlacement
-  windowToolbar 

Type Property

# windowToolbar

The placement for the containing window’s toolbar, sometimes referred to as the titlebar.

macOS 13.0+

``` source
static var windowToolbar: ToolbarPlacement { get }
```

## Discussion

When hidden using toolbar(_:for:), this hides the entire window toolbar, including the title and “traffic light” window controls. To remove the custom toolbar item content only, use automatic.

Use toolbarBackground(_:for:) to hide the background of the window toolbar.

## See Also

### Getting placements

static var automatic: ToolbarPlacement

The primary toolbar.

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

