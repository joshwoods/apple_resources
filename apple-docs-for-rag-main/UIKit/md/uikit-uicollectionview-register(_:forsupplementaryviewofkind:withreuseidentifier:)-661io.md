

- UIKit
- UICollectionView
-  register(\_:forSupplementaryViewOfKind:withReuseIdentifier:) 

Instance Method

# register(\_:forSupplementaryViewOfKind:withReuseIdentifier:)

Registers a class for use in creating supplementary views for the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func register(
    _ viewClass: AnyClass?,
    forSupplementaryViewOfKind elementKind: String,
    withReuseIdentifier identifier: String
)
```

## Parameters 

`viewClass`  

The class to use for the supplementary view.

`elementKind`  

The kind of supplementary view to create. This value is defined by the layout object. This parameter must not be `nil`.

`identifier`  

The reuse identifier to associate with the specified class. This parameter must not be `nil` and must not be an empty string.

## Discussion

Prior to calling the dequeueReusableSupplementaryView(ofKind:withReuseIdentifier:for:) method of the collection view, you must use this method or the register(_:forSupplementaryViewOfKind:withReuseIdentifier:) method to tell the collection view how to create a supplementary view of the given type. If a view of the specified type isn’t currently in a reuse queue, the collection view uses the provided information to create a view object automatically.

If you previously registered a class or nib file with the same element kind and reuse identifier, the class you specify in the `viewClass` parameter replaces the old entry. You may specify `nil` for `viewClass` if you want to unregister the class from the specified element kind and reuse identifier.

## See Also

### Creating headers and footers

struct SupplementaryRegistration

A registration for the collection view’s supplementary views.

func dequeueConfiguredReusableSupplementary&lt;Supplementary>(using: UICollectionView.SupplementaryRegistration&lt;Supplementary>, for: IndexPath) -> Supplementary

Dequeues a configured reusable supplementary view object.

func register(UINib?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a nib file for use in creating supplementary views for the collection view.

func dequeueReusableSupplementaryView(ofKind: String, withReuseIdentifier: String, for: IndexPath) -> UICollectionReusableView

Dequeues a reusable supplementary view located by its identifier and kind.

