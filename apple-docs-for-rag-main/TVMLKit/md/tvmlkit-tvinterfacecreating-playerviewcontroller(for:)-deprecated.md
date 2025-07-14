

- TVMLKit
- TVInterfaceCreating
-  playerViewController(for:) Deprecated

Instance Method

# playerViewController(for:)

Returns the custom player user interface for a custom player.

tvOS 12.0–18.0Deprecated

``` source
optional func playerViewController(for player: TVPlayer) -> UIViewController?
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`player`  

The player requesting a view controller.

## Return Value

The new view controller associated with the view element. If the app doesn’t handle this event, you must return nil.

## See Also

### Updating View Information

func makeViewController(element: TVViewElement, existingViewController: UIViewController?) -> UIViewController?

Returns a view controller for a view element.

Deprecated

func makeView(element: TVViewElement, existingView: UIView?) -> UIView?

Returns a view for a view element.

Deprecated

func collectionViewCellClass(for: TVViewElement) -> AnyClass?

Returns a collection view cell for the specified element.

Deprecated

