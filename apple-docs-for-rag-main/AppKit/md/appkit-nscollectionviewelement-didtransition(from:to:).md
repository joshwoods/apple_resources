

- AppKit
- NSCollectionViewElement
-  didTransition(from:to:) 

Instance Method

# didTransition(from:to:)

Tells the element that the layout object of the collection view changed.

macOS 10.11+

``` source
@MainActor
optional func didTransition(
    from oldLayout: NSCollectionViewLayout,
    to newLayout: NSCollectionViewLayout
)
```

## Parameters 

`oldLayout`  

The collection view’s previous layout object.

`newLayout`  

The current layout object associated with the collection view.

## Discussion

The default implementation of this method does nothing. Subclasses can override it and use it to finalize any behaviors associated with the change in layouts.

### Special Considerations

In OS X 10.11, this method is never called.

## See Also

### Managing Layout Changes

func preferredLayoutAttributesFitting(NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutAttributes

Asks your element if it wants to modify any layout attributes before they are applied.

func apply(NSCollectionViewLayoutAttributes)

Applies the specified layout attributes to the element.

func willTransition(from: NSCollectionViewLayout, to: NSCollectionViewLayout)

Tells the element that the layout object of the collection view is about to change.

