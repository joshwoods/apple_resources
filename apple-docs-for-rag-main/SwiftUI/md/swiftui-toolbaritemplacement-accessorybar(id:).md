

- SwiftUI
- ToolbarItemPlacement
-  accessoryBar(id:) 

Type Method

# accessoryBar(id:)

Creates a unique accessory bar placement.

macOS 13.0+

``` source
@backDeployed(before: macOS 14.0)
static func accessoryBar(id: ID) -> ToolbarItemPlacement where ID : Hashable
```

## Parameters 

`id`  

A unique identifier for this placement.

## Discussion

On macOS, items with an accessory bar placement are placed in a section below the title bar and toolbar area of the window. Each separate identifier will correspond to a separate accessory bar that is added to this area.

```
extension ToolbarItemPlacement {
    static let favoritesBar = accessoryBar(id: "com.example.favorites")
}
...
BrowserView()
    .toolbar {
        ToolbarItem(placement: .favoritesBar) {
            FavoritesBar()
        }
    }
```

## See Also

### Getting explicit placement

static var topBarLeading: ToolbarItemPlacement

Places the item in the leading edge of the top bar.

static var topBarTrailing: ToolbarItemPlacement

Places the item in the trailing edge of the top bar.

static let bottomBar: ToolbarItemPlacement

Places the item in the bottom toolbar.

static let bottomOrnament: ToolbarItemPlacement

Places the item in an ornament under the window.

static let keyboard: ToolbarItemPlacement

The item is placed in the keyboard section.

