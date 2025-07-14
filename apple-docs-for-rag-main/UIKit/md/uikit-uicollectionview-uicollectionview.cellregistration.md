

- UIKit
- UICollectionView
-  UICollectionView.CellRegistration 

Structure

# UICollectionView.CellRegistration

A registration for the collection view’s cells.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct CellRegistration where Cell : UICollectionViewCell
```

## Overview

Use a cell registration to register cells with your collection view and configure each cell for display. You create a cell registration with your cell type and data item type as the registration’s generic parameters, passing in a registration handler to configure the cell. In the registration handler, you specify how to configure the content and appearance of that type of cell.

The following example creates a cell registration for cells of type UICollectionViewListCell. It creates a content configuration with a system default style, customizes the content and appearance of the configuration, and then assigns the configuration to the cell.

```
let cellRegistration = UICollectionView.CellRegistration { cell, indexPath, item in

    var contentConfiguration = cell.defaultContentConfiguration()

    contentConfiguration.text = "\(item)"
    contentConfiguration.textProperties.color = .lightGray

    cell.contentConfiguration = contentConfiguration
}
```

After you create a cell registration, you pass it in to dequeueConfiguredReusableCell(using:for:item:), which you call from your data source’s cell provider.

```
dataSource = UICollectionViewDiffableDataSource(collectionView: collectionView) {
    (collectionView: UICollectionView, indexPath: IndexPath, itemIdentifier: Int) -> UICollectionViewCell? in

    return collectionView.dequeueConfiguredReusableCell(using: cellRegistration,
                                                        for: indexPath,
                                                        item: itemIdentifier)
}
```

You don’t need to call register(_:forCellWithReuseIdentifier:) or register(_:forCellWithReuseIdentifier:). The collection view registers your cell automatically when you pass the cell registration to dequeueConfiguredReusableCell(using:for:item:).

Important

Don’t create your cell registration inside a UICollectionViewDiffableDataSource.CellProvider closure; doing so prevents cell reuse, and generates an exception in iOS 15 and higher.

## Topics

### Creating a cell registration

init(handler: UICollectionView.CellRegistration&lt;Cell, Item>.Handler)

Creates a cell registration with the specified registration handler.

init(cellNib: UINib, handler: UICollectionView.CellRegistration&lt;Cell, Item>.Handler)

Creates a cell registration with the specified registration handler and nib file.

typealias Handler

A closure that handles the cell registration and configuration.

## See Also

### Creating cells

func dequeueConfiguredReusableCell&lt;Cell, Item>(using: UICollectionView.CellRegistration&lt;Cell, Item>, for: IndexPath, item: Item?) -> Cell

Dequeues a configured reusable cell object.

func register(AnyClass?, forCellWithReuseIdentifier: String)

Registers a class for use in creating new collection view cells.

func register(UINib?, forCellWithReuseIdentifier: String)

Registers a nib file for use in creating new collection view cells.

func dequeueReusableCell(withReuseIdentifier: String, for: IndexPath) -> UICollectionViewCell

Dequeues a reusable cell object located by its identifier.

