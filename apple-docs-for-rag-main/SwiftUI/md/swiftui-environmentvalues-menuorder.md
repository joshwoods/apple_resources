

- SwiftUI
- EnvironmentValues
-  menuOrder 

Instance Property

# menuOrder

The preferred order of items for menus presented from this view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var menuOrder: MenuOrder { get set }
```

## Discussion

Set this value for a view hierarchy by calling the menuOrder(_:) view modifier.

## See Also

### Setting a preferred order

func menuOrder(MenuOrder) -> some View

Sets the preferred order of items for menus presented from this view.

struct MenuOrder

The order in which a menu presents its content.

