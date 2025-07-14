

- AppKit
- NSCollectionViewLayout
-  shouldInvalidateLayout(forPreferredLayoutAttributes:withOriginalAttributes:) 

Instance Method

# shouldInvalidateLayout(forPreferredLayoutAttributes:withOriginalAttributes:)

Returns a Boolean indicating whether changes to a cell’s layout attributes trigger a larger layout update.

macOS

``` source
@MainActor
func shouldInvalidateLayout(
    forPreferredLayoutAttributes preferredAttributes: NSCollectionViewLayoutAttributes,
    withOriginalAttributes originalAttributes: NSCollectionViewLayoutAttributes
) -> Bool
```

## Parameters 

`preferredAttributes`  

The preferred layout attributes of an element.

`originalAttributes`  

The attributes that the layout object originally suggested for the item.

## Return Value

true if the layout should be invalidated or false if it should not.

## Discussion

The default implementation of this method returns NO to indicate that layout is not needed. You can override this method in your custom layout classes and return a different value as needed. Your implementation of this method should determine if the new attributes would cause changes to the layout of other portions of the collection view.

If you return true from this method, the collection view invalidates the layout using the invalidateLayout(with:) method. The invalidation context passed to that method is created using the invalidationContext(forPreferredLayoutAttributes:withOriginalAttributes:) method.

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

func invalidationContext(forBoundsChange: NSRect) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

func invalidationContext(forPreferredLayoutAttributes: NSCollectionViewLayoutAttributes, withOriginalAttributes: NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutInvalidationContext

Returns an invalidation context object that defines the portions of the layout that need to be updated.

