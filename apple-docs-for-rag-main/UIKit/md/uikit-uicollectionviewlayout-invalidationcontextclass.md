

- UIKit
- UICollectionViewLayout
-  invalidationContextClass 

Type Property

# invalidationContextClass

Returns the class to use when creating an invalidation context for the layout.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class var invalidationContextClass: AnyClass { get }
```

## Discussion

If you subclass `UICollectionViewLayout` and use a custom invalidation context object to improve the performance of your layout updates, override this method and return your UICollectionViewLayoutInvalidationContext subclass. When the collection view needs to invalidate your layout, it uses the class you provide to create an appropriate invalidation context object.

## See Also

### Invalidating the layout

func invalidateLayout()

Invalidates the current layout and triggers a layout update.

func invalidateLayout(with: UICollectionViewLayoutInvalidationContext)

Invalidates the current layout using the information in the provided context object.

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

