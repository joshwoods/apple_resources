

- UIKit
- UICollectionView
-  dequeueReusableCell(withReuseIdentifier:for:) 

Instance Method

# dequeueReusableCell(withReuseIdentifier:for:)

Dequeues a reusable cell object located by its identifier.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dequeueReusableCell(
    withReuseIdentifier identifier: String,
    for indexPath: IndexPath
) -> UICollectionViewCell
```

## Parameters 

`identifier`  

The reuse identifier for the specified cell. This parameter must not be `nil`.

`indexPath`  

The index path specifying the location of the cell. The data source receives this information when it is asked for the cell and should just pass it along. This method uses the index path to perform additional configuration based on the cell’s position in the collection view.

## Return Value

A valid UICollectionReusableView object.

## Discussion

Call this method from your data source object when asked to provide a new cell for the collection view. This method dequeues an existing cell if one is available or creates a new one based on the class or nib file you previously registered.

Important

You must register a class or nib file using the register(_:forCellWithReuseIdentifier:) or register(_:forCellWithReuseIdentifier:) method before calling this method.

If you registered a class for the specified `identifier` and a new cell must be created, this method initializes the cell by calling its init(frame:) method. For nib-based cells, this method loads the cell object from the provided nib file. If an existing cell was available for reuse, this method calls the cell’s prepareForReuse() method instead.

## See Also

### Creating cells

struct CellRegistration

A registration for the collection view’s cells.

func dequeueConfiguredReusableCell&lt;Cell, Item>(using: UICollectionView.CellRegistration&lt;Cell, Item>, for: IndexPath, item: Item?) -> Cell

Dequeues a configured reusable cell object.

func register(AnyClass?, forCellWithReuseIdentifier: String)

Registers a class for use in creating new collection view cells.

func register(UINib?, forCellWithReuseIdentifier: String)

Registers a nib file for use in creating new collection view cells.

