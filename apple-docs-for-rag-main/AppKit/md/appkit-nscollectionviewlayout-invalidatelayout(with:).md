

- AppKit
- NSCollectionViewLayout
-  invalidateLayout(with:) 

Instance Method

# invalidateLayout(with:)

Invalidates specific parts of the layout using the specified context object.

macOS 10.11+

``` source
@MainActor
func invalidateLayout(with context: NSCollectionViewLayoutInvalidationContext)
```

## Parameters 

`context`  

The context object indicating which parts of the layout need to be updated.

## Discussion

Call this method when you make changes that need to be reflected by the collection view, but which do not require the replacement of all of the layout information. You use this method to minimize the work performed by the layout object. Instead of optimizing everything, the specified context object indicates which parts of the layout need to be recomputed. All other layout information is left alone.

When implementing a custom layout, you can override this method and use it to process information provided by a custom invalidation context. You are not required to provide a custom invalidation context but might do so if you are able to provide additional properties that can help optimize layout updates. If you override this method, you must call `super` at some point in your implementation.

## See Also

### Invalidating the Layout

func invalidateLayout()

Invalidates all layout information and triggers a layout update.

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

