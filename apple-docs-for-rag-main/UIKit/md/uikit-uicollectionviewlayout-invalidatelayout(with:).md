

- UIKit
- UICollectionViewLayout
-  invalidateLayout(with:) 

Instance Method

# invalidateLayout(with:)

Invalidates the current layout using the information in the provided context object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func invalidateLayout(with context: UICollectionViewLayoutInvalidationContext)
```

## Parameters 

`context`  

The context object indicating which parts of the layout to refresh.

## Discussion

The default implementation of this method optimizes the layout process using the base properties of the UICollectionViewLayoutInvalidationContext class. If you define a custom context object for your layout, override this method and apply any custom properties of the context object to your layout computations.

If you override this method, you must call `super` at some point in your implementation.

## See Also

### Invalidating the layout

func invalidateLayout()

Invalidates the current layout and triggers a layout update.

class var invalidationContextClass: AnyClass

Returns the class to use when creating an invalidation context for the layout.

func shouldInvalidateLayout(forBoundsChange: CGRect) -> Bool

Asks the layout object if the new bounds require a layout update.

func invalidationContext(forBoundsChange: CGRect) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that defines the portions of the layout that should change when a bounds change occurs.

func shouldInvalidateLayout(forPreferredLayoutAttributes: UICollectionViewLayoutAttributes, withOriginalAttributes: UICollectionViewLayoutAttributes) -> Bool

Asks the layout object if changes to a self-sizing cell require a layout update.

func invalidationContext(forPreferredLayoutAttributes: UICollectionViewLayoutAttributes, withOriginalAttributes: UICollectionViewLayoutAttributes) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that identifies the portions of the layout that should change in response to dynamic cell changes.

func invalidationContext(forInteractivelyMovingItems: [IndexPath], withTargetPosition: CGPoint, previousIndexPaths: [IndexPath], previousPosition: CGPoint) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that identifies the items that are being interactively moved in the layout.

func invalidationContextForEndingInteractiveMovementOfItems(toFinalIndexPaths: [IndexPath], previousIndexPaths: [IndexPath], movementCancelled: Bool) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that identifies the items that were moved

