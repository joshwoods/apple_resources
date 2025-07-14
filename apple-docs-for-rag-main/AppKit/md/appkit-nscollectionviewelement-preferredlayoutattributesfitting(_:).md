

- AppKit
- NSCollectionViewElement
-  preferredLayoutAttributesFitting(\_:) 

Instance Method

# preferredLayoutAttributesFitting(\_:)

Asks your element if it wants to modify any layout attributes before they are applied.

macOS 10.11+

``` source
@MainActor
optional func preferredLayoutAttributesFitting(_ layoutAttributes: NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutAttributes
```

## Parameters 

`layoutAttributes`  

The attributes provided by the layout object. These attributes represent the values that the layout object intends to apply to the element.

## Return Value

The final attributes to apply to the element.

## Discussion

The default implementation of this method returns the same attributes that are in the `layoutAttributes` parameter. You can override this method in subclasses and use it to return a different set of attributes. If you override this method, call `super` first to give the system the opportunity to make changes, then modify the returned attributes.

### Special Considerations

In OS X 10.11, this method is never called.

## See Also

### Managing Layout Changes

func apply(NSCollectionViewLayoutAttributes)

Applies the specified layout attributes to the element.

func willTransition(from: NSCollectionViewLayout, to: NSCollectionViewLayout)

Tells the element that the layout object of the collection view is about to change.

func didTransition(from: NSCollectionViewLayout, to: NSCollectionViewLayout)

Tells the element that the layout object of the collection view changed.

