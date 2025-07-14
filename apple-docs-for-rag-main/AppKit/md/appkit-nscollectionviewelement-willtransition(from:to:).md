

- AppKit
- NSCollectionViewElement
-  willTransition(from:to:) 

Instance Method

# willTransition(from:to:)

Tells the element that the layout object of the collection view is about to change.

macOS 10.11+

``` source
@MainActor
optional func willTransition(
    from oldLayout: NSCollectionViewLayout,
    to newLayout: NSCollectionViewLayout
)
```

## Parameters 

`oldLayout`  

The current layout object used by the collection view.

`newLayout`  

The new layout object that is about to be used by the collection view.

## Discussion

The default implementation of this method does nothing. Subclasses can override it and use it to prepare for the change in layouts.

### Special Considerations

In OS X 10.11, this method is never called.

## See Also

### Managing Layout Changes

func preferredLayoutAttributesFitting(NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutAttributes

Asks your element if it wants to modify any layout attributes before they are applied.

func apply(NSCollectionViewLayoutAttributes)

Applies the specified layout attributes to the element.

func didTransition(from: NSCollectionViewLayout, to: NSCollectionViewLayout)

Tells the element that the layout object of the collection view changed.

