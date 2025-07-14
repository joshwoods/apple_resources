

- AppKit
- NSCollectionViewLayout
-  invalidationContextClass 

Type Property

# invalidationContextClass

Returns the class to use when creating an invalidation context object for the layout.

macOS

``` source
@MainActor
class var invalidationContextClass: AnyClass { get }
```

## Return Value

A custom class that descends from NSCollectionViewLayoutInvalidationContext.

## Discussion

If you define a custom invalidation context class to store information related to your layout, override this method and use it to return your custom subclass. Methods of this class that create invalidation contexts automatically create instances of the class you provide, initializing those instances using its init() method.

## See Also

### Invalidating the Layout

func invalidateLayout()

Invalidates all layout information and triggers a layout update.

func invalidateLayout(with: NSCollectionViewLayoutInvalidationContext)

Invalidates specific parts of the layout using the specified context object.

func shouldInvalidateLayout(forBoundsChange: NSRect) -> Bool

Returns a Boolean indicating whether a bounds change triggers a layout update.

func shouldInvalidateLayout(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> Bool

Returns a Boolean indicating whether changes to a cell’s layout attributes trigger a larger layout update.

func invalidationContext(forBoundsChange: NSRect) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

func invalidationContext(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

