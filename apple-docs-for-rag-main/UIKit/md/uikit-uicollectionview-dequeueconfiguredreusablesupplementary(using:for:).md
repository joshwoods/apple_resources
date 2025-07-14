

- UIKit
- UICollectionView
-  dequeueConfiguredReusableSupplementary(using:for:) 

Instance Method

# dequeueConfiguredReusableSupplementary(using:for:)

Dequeues a configured reusable supplementary view object.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
func dequeueConfiguredReusableSupplementary(
    using registration: UICollectionView.SupplementaryRegistration,
    for indexPath: IndexPath
) -> Supplementary where Supplementary : UICollectionReusableView
```

## Parameters 

`registration`  

The supplementary registration for configuring the supplementary view object. See UICollectionView.SupplementaryRegistration.

`indexPath`  

The index path that specifies the location of the supplementary view in the collection view.

## Return Value

A configured reusable supplementary view object.

## See Also

### Creating headers and footers

struct SupplementaryRegistration

A registration for the collection view’s supplementary views.

func register(AnyClass?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a class for use in creating supplementary views for the collection view.

func register(UINib?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a nib file for use in creating supplementary views for the collection view.

func dequeueReusableSupplementaryView(ofKind: String, withReuseIdentifier: String, for: IndexPath) -> UICollectionReusableView

Dequeues a reusable supplementary view located by its identifier and kind.

