

- SwiftUI
- MenuOrder
-  automatic 

Type Property

# automatic

The ordering of the menu chosen by the system for the current context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static let automatic: MenuOrder
```

## Discussion

On iOS, this order resolves to fixed for menus presented within scrollable content. Pickers that use the menu style also default to fixed order. In all other cases, menus default to priority order.

On macOS, tvOS and watchOS, the `automatic` order always resolves to fixed order.

## See Also

### Getting menu orders

static let fixed: MenuOrder

Order items from top to bottom.

static let priority: MenuOrder

Keep the first items closest to user’s interaction point.

