

- TVMLKit
- TVInterfaceCreating
-  collectionViewCellClass(for:) Deprecated

Instance Method

# collectionViewCellClass(for:)

Returns a collection view cell for the specified element.

tvOS 9.0–18.0Deprecated

``` source
optional func collectionViewCellClass(for element: TVViewElement) -> AnyClass?
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`element`  

The element a collection view cell is created for.

## Return Value

The new collection view cell associated with the given element name.

## Discussion

The collection view cell must be in a list, shelf, or grid. This method is called once per unique element name as a common cell class is used for all elements that share the same name in a collection. Return `nil` for default handling.

## See Also

### Updating View Information

func makeViewController(element: TVViewElement, existingViewController: UIViewController?) -> UIViewController?

Returns a view controller for a view element.

Deprecated

func makeView(element: TVViewElement, existingView: UIView?) -> UIView?

Returns a view for a view element.

Deprecated

func playerViewController(for: TVPlayer) -> UIViewController?

Returns the custom player user interface for a custom player.

Deprecated

