

- AppKit
- NSCollectionViewElement
-  apply(\_:) 

Instance Method

# apply(\_:)

Applies the specified layout attributes to the element.

macOS 10.11+

``` source
@MainActor
optional func apply(_ layoutAttributes: NSCollectionViewLayoutAttributes)
```

## Parameters 

`layoutAttributes`  

The layout attributes to apply.

## Discussion

In your custom elements, you can use this method to apply the specified attributes to your content. For example, if your element object is a view controller, you would override this method and use it to apply the attributes to the root view object. When using your element with a layout object that supports custom attributes, you would also use this method to apply those custom attributes.

## See Also

### Managing Layout Changes

func preferredLayoutAttributesFitting(NSCollectionViewLayoutAttributes) -> NSCollectionViewLayoutAttributes

Asks your element if it wants to modify any layout attributes before they are applied.

func willTransition(from: NSCollectionViewLayout, to: NSCollectionViewLayout)

Tells the element that the layout object of the collection view is about to change.

func didTransition(from: NSCollectionViewLayout, to: NSCollectionViewLayout)

Tells the element that the layout object of the collection view changed.

