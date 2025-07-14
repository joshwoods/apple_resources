

- AppKit
- NSCollectionViewLayout
-  invalidateLayout() 

Instance Method

# invalidateLayout()

Invalidates all layout information and triggers a layout update.

macOS 10.11+

``` source
@MainActor
func invalidateLayout()
```

## Discussion

Call this method when you make changes that require updating all of the current layout information. This method marks the layout as invalid and returns right away, so you can call this method multiple times from the same block of code without triggering multiple layout updates. During the next update cycle, the collection view requests new layout information and updates its contents accordingly.

If you override this method, you must call `super` at some point in your implementation.

## See Also

### Invalidating the Layout

func invalidateLayout(with: NSCollectionViewLayoutInvalidationContext)

Invalidates specific parts of the layout using the specified context object.

class var invalidationContextClass: AnyClass

Returns the class to use when creating an invalidation context object for the layout.

func shouldInvalidateLayout(forBoundsChange: NSRect) -> Bool

Returns a Boolean indicating whether a bounds change triggers a layout update.

func shouldInvalidateLayout(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> Bool

Returns a Boolean indicating whether changes to a cell’s layout attributes trigger a larger layout update.

func invalidationContext(forBoundsChange: NSRect) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

func invalidationContext(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

