

- UIKit
- UICollectionViewLayout
-  invalidationContext(forInteractivelyMovingItems:withTargetPosition:previousIndexPaths:previousPosition:) 

Instance Method

# invalidationContext(forInteractivelyMovingItems:withTargetPosition:previousIndexPaths:previousPosition:)

Retrieves a context object that identifies the items that are being interactively moved in the layout.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func invalidationContext(
    forInteractivelyMovingItems targetIndexPaths: [IndexPath],
    withTargetPosition targetPosition: CGPoint,
    previousIndexPaths: [IndexPath],
    previousPosition: CGPoint
) -> UICollectionViewLayoutInvalidationContext
```

## Parameters 

`targetIndexPaths`  

The current locations of the items being moved.

`targetPosition`  

The point in the collection view’s coordinate system that is the potential drop point for the items.

`previousIndexPaths`  

The previous locations of the items being moved.

`previousPosition`  

The previous point in the collection view’s coordinate system. This is the point that was previously used to determine the drop point for the items.

## Return Value

An invalidation context that includes information about what changes need to be made to the layout.

## Discussion

The layout object uses this method to retrieve invalidation contexts when an interactive move of one or more items is in progress. The default implementation creates an instance of the class provided by the invalidationContextClass class method, fills it with the provided information, and returns it. If you want to use a custom invalidation context object with your layout, always override that method and return your custom class.

Subclasses can override this method and use it to perform additional configuration of the invalidation context before returning it. In your custom implementation, call `super` so that the parent class can perform the basic configuration of the object.

## See Also

### Invalidating the layout

func invalidateLayout()

Invalidates the current layout and triggers a layout update.

func invalidateLayout(with: UICollectionViewLayoutInvalidationContext)

Invalidates the current layout using the information in the provided context object.

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

func invalidationContextForEndingInteractiveMovementOfItems(toFinalIndexPaths: [IndexPath], previousIndexPaths: [IndexPath], movementCancelled: Bool) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that identifies the items that were moved

