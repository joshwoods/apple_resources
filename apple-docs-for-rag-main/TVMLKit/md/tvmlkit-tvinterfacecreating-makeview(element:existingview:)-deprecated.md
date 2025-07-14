

- TVMLKit
- TVInterfaceCreating
-  makeView(element:existingView:) Deprecated

Instance Method

# makeView(element:existingView:)

Returns a view for a view element.

tvOS 9.0–18.0Deprecated

``` source
optional func makeView(
    element: TVViewElement,
    existingView: UIView?
) -> UIView?
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`element`  

The view element requesting a new view.

`existingView`  

The current view.

## Return Value

The new view associated with the view element. If the app doesn’t handle the event, you must return `nil`.

## Mentioned in 

Creating TVML Elements

## Discussion

When possible, update the view contained in the `existingView` parameter instead of creating a new view. However, if the existing view is an instance of UICollectionViewCell, you must configure the cell instead of creating a new instance.

## See Also

### Updating View Information

func makeViewController(element: TVViewElement, existingViewController: UIViewController?) -> UIViewController?

Returns a view controller for a view element.

Deprecated

func collectionViewCellClass(for: TVViewElement) -> AnyClass?

Returns a collection view cell for the specified element.

Deprecated

func playerViewController(for: TVPlayer) -> UIViewController?

Returns the custom player user interface for a custom player.

Deprecated

