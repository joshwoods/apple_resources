

- TVMLKit
- TVInterfaceCreating
-  makeViewController(element:existingViewController:) Deprecated

Instance Method

# makeViewController(element:existingViewController:)

Returns a view controller for a view element.

tvOS 9.0–18.0Deprecated

``` source
optional func makeViewController(
    element: TVViewElement,
    existingViewController: UIViewController?
) -> UIViewController?
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`element`  

The view element requesting a view controller.

`existingViewController`  

The current view controller.

## Return Value

The new view controller associated with the view element. If the app doesn’t handle this event, you must return `nil`.

## Discussion

When possible, update the view controller contained in the `existingViewController` parameter instead of creating a new view controller.

## See Also

### Updating View Information

func makeView(element: TVViewElement, existingView: UIView?) -> UIView?

Returns a view for a view element.

Deprecated

func collectionViewCellClass(for: TVViewElement) -> AnyClass?

Returns a collection view cell for the specified element.

Deprecated

func playerViewController(for: TVPlayer) -> UIViewController?

Returns the custom player user interface for a custom player.

Deprecated

