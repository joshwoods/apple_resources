

- UIKit
- UICollectionView
-  dequeueConfiguredReusableCell(using:for:item:) 

Instance Method

# dequeueConfiguredReusableCell(using:for:item:)

Dequeues a configured reusable cell object.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
func dequeueConfiguredReusableCell(
    using registration: UICollectionView.CellRegistration,
    for indexPath: IndexPath,
    item: Item?
) -> Cell where Cell : UICollectionViewCell
```

## Parameters 

`registration`  

The cell registration for configuring the cell object. See UICollectionView.CellRegistration.

`indexPath`  

The index path that specifies the location of the cell in the collection view.

`item`  

The item that provides data for the cell.

## Return Value

A configured reusable cell object.

## See Also

### Creating cells

struct CellRegistration

A registration for the collection view’s cells.

func register(AnyClass?, forCellWithReuseIdentifier: String)

Registers a class for use in creating new collection view cells.

func register(UINib?, forCellWithReuseIdentifier: String)

Registers a nib file for use in creating new collection view cells.

func dequeueReusableCell(withReuseIdentifier: String, for: IndexPath) -> UICollectionViewCell

Dequeues a reusable cell object located by its identifier.

