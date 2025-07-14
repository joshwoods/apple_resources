

- AppKit
- NSCollectionViewLayout
-  invalidationContext(forBoundsChange:) 

Instance Method

# invalidationContext(forBoundsChange:)

Returns an invalidation context object that defines the portions of the layout that need to be updated.

macOS

``` source
@MainActor
func invalidationContext(forBoundsChange newBounds: NSRect) -> NSCollectionViewLayoutInvalidationContext
```

## Parameters 

`newBounds`  

The new bounds for the collection view.

## Return Value

An invalidation context that describes the changes to be made. This value is never `nil`.

## Discussion

The default implementation of this method creates an instance of the class returned by the invalidationContextClass method and initializes it using its init() method. Subclasses can override this method and configure additional properties of the invalidation context. In your implementation, you must call `super` first to get the context object; you can then configure that object and return it.

## See Also

### Invalidating the Layout

func invalidateLayout()

Invalidates all layout information and triggers a layout update.

func invalidateLayout(with: NSCollectionViewLayoutInvalidationContext)

Invalidates specific parts of the layout using the specified context object.

class var invalidationContextClass: AnyClass

Returns the class to use when creating an invalidation context object for the layout.

func shouldInvalidateLayout(forBoundsChange: NSRect) -> Bool

Returns a Boolean indicating whether a bounds change triggers a layout update.

func shouldInvalidateLayout(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> Bool

Returns a Boolean indicating whether changes to a cell’s layout attributes trigger a larger layout update.

func invalidationContext(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

