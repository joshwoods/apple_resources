

- UIKit
- UICollectionView
-  UICollectionView.SupplementaryRegistration 

Structure

# UICollectionView.SupplementaryRegistration

A registration for the collection view’s supplementary views.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct SupplementaryRegistration where Supplementary : UICollectionReusableView
```

## Overview

Use a supplementary registration to register supplementary views, like headers and footers, with your collection view and configure each view for display. You create a supplementary registration with your supplementary view type and data item type as the registration’s generic parameters, passing in a registration handler to configure the view. In the registration handler, you specify how to configure the content and appearance of that type of supplementary view.

The following example creates a supplementary registration for a custom header view subclass.

```
let headerRegistration = UICollectionView.SupplementaryRegistration
    (elementKind: "Header") {
    supplementaryView, string, indexPath in
    supplementaryView.label.text = "\(string) for section \(indexPath.section)"
    supplementaryView.backgroundColor = .lightGray
}
```

After you create a supplementary registration, you pass it in to dequeueConfiguredReusableSupplementary(using:for:), which you call from your data source’s supplementaryViewProvider.

```
dataSource.supplementaryViewProvider = { collectionView, elementKind, indexPath in
    return collectionView.dequeueConfiguredReusableSupplementary(using: headerRegistration,
                                                                 for: indexPath)
}
```

You don’t need to call register(_:forSupplementaryViewOfKind:withReuseIdentifier:) or register(_:forSupplementaryViewOfKind:withReuseIdentifier:). The registration occurs automatically when you pass the supplementary view registration to dequeueConfiguredReusableSupplementary(using:for:).

Important

Don’t create your supplementary view registration inside a UICollectionViewDiffableDataSource.SupplementaryViewProvider closure; doing so prevents reuse, and generates an exception in iOS 15 and higher.

## Topics

### Creating a supplementary registration

init(elementKind: String, handler: UICollectionView.SupplementaryRegistration&lt;Supplementary>.Handler)

Creates a supplementary registration for the specified element kind with a registration handler.

init(supplementaryNib: UINib, elementKind: String, handler: UICollectionView.SupplementaryRegistration&lt;Supplementary>.Handler)

Creates a supplementary registration for the specified element kind with a registration handler and nib file.

typealias Handler

A closure that handles the supplementary view registration and configuration.

## See Also

### Creating headers and footers

func dequeueConfiguredReusableSupplementary&lt;Supplementary>(using: UICollectionView.SupplementaryRegistration&lt;Supplementary>, for: IndexPath) -> Supplementary

Dequeues a configured reusable supplementary view object.

func register(AnyClass?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a class for use in creating supplementary views for the collection view.

func register(UINib?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a nib file for use in creating supplementary views for the collection view.

func dequeueReusableSupplementaryView(ofKind: String, withReuseIdentifier: String, for: IndexPath) -> UICollectionReusableView

Dequeues a reusable supplementary view located by its identifier and kind.

