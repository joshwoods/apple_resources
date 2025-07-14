

- SwiftUI
- ToolbarPlacement
-  accessoryBar(id:) 

Type Method

# accessoryBar(id:)

Creates a unique accessory bar placement.

macOS 13.0+

``` source
@backDeployed(before: macOS 14.0)
static func accessoryBar(id: ID) -> ToolbarPlacement where ID : Hashable
```

## Parameters 

`id`  

A unique identifier for this placement.

## Discussion

On macOS, accessory bars are in a section below the title bar and toolbar area of the window. Each separate identifier will correspond to a separate accessory bar that is added to this area.

Use a custom placement to control the appearance of the containing bar for items using a custom ToolbarItemPlacement with the same identifier.

```
private let favoritesBarID = "com.example.favoritesBar"
extension ToolbarItemPlacement {
    static let favoritesBar = accessoryBar(id: favoritesBarID)
}
extension ToolbarPlacement {
    static let favoritesBar = accessoryBar(id: favoritesBarID)
}
...
BrowserView()
    .toolbar {
        ToolbarItem(placement: .favoritesBar) {
            FavoritesBar()
        }
    }
    .toolbar(.hidden, for: .favoritesBar)
```

## See Also

### Getting placements

static var automatic: ToolbarPlacement

The primary toolbar.

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

