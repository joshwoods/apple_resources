

- UIKit
- UICollectionView
-  register(\_:forCellWithReuseIdentifier:) 

Instance Method

# register(\_:forCellWithReuseIdentifier:)

Registers a nib file for use in creating new collection view cells.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func register(
    _ nib: UINib?,
    forCellWithReuseIdentifier identifier: String
)
```

## Parameters 

`nib`  

The nib object containing the cell object. The nib file must contain only one top-level object and that object must be of the type UICollectionViewCell.

`identifier`  

The reuse identifier to associate with the specified nib file. This parameter must not be `nil` and must not be an empty string.

## Discussion

Prior to calling the dequeueReusableCell(withReuseIdentifier:for:) method of the collection view, you must use this method or the register(_:forCellWithReuseIdentifier:) method to tell the collection view how to create a new cell of the given type. If a cell of the specified type is not currently in a reuse queue, the collection view uses the provided information to create a new cell object automatically.

If you previously registered a class or nib file with the same reuse identifier, the object you specify in the `nib` parameter replaces the old entry. You may specify `nil` for `nib` if you want to unregister the nib file from the specified reuse identifier.

## See Also

### Creating cells

struct CellRegistration

A registration for the collection view’s cells.

func dequeueConfiguredReusableCell&lt;Cell, Item>(using: UICollectionView.CellRegistration&lt;Cell, Item>, for: IndexPath, item: Item?) -> Cell

Dequeues a configured reusable cell object.

func register(AnyClass?, forCellWithReuseIdentifier: String)

Registers a class for use in creating new collection view cells.

func dequeueReusableCell(withReuseIdentifier: String, for: IndexPath) -> UICollectionViewCell

Dequeues a reusable cell object located by its identifier.

