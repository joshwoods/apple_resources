

- AppKit
- NSCollectionViewLayout
-  shouldInvalidateLayout(forBoundsChange:) 

Instance Method

# shouldInvalidateLayout(forBoundsChange:)

Returns a Boolean indicating whether a bounds change triggers a layout update.

macOS

``` source
@MainActor
func shouldInvalidateLayout(forBoundsChange newBounds: NSRect) -> Bool
```

## Parameters 

`newBounds`  

The new bounds of the collection view.

## Return Value

true if a layout should be invalidated or false if the layout is still valid.

## Discussion

The default implementation of this method returns false. You can override this method in your custom layout classes and return a different value as needed. Your implementation of the method should determine if the new bounds would cause changes to the layout of other portions of the collection view.

If you return true from this method, the collection view invalidates the layout using the invalidateLayout(with:) method. The invalidation context passed to that method is created using the invalidationContext(forBoundsChange:) method.

## See Also

### Invalidating the Layout

func invalidateLayout()

Invalidates all layout information and triggers a layout update.

func invalidateLayout(with: NSCollectionViewLayoutInvalidationContext)

Invalidates specific parts of the layout using the specified context object.

class var invalidationContextClass: AnyClass

Returns the class to use when creating an invalidation context object for the layout.

func shouldInvalidateLayout(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> Bool

Returns a Boolean indicating whether changes to a cell’s layout attributes trigger a larger layout update.

func invalidationContext(forBoundsChange: NSRect) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

func invalidationContext(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

