

- UIKit
- UICollectionView
-  register(\_:forCellWithReuseIdentifier:) 

Instance Method

# register(\_:forCellWithReuseIdentifier:)

Registers a class for use in creating new collection view cells.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func register(
    _ cellClass: AnyClass?,
    forCellWithReuseIdentifier identifier: String
)
```

## Parameters 

`cellClass`  

The class of a cell that you want to use in the collection view.

`identifier`  

The reuse identifier to associate with the specified class. This parameter must not be `nil` and must not be an empty string.

## Discussion

Prior to calling the dequeueReusableCell(withReuseIdentifier:for:) method of the collection view, you must use this method or the register(_:forCellWithReuseIdentifier:) method to tell the collection view how to create a new cell of the given type. If a cell of the specified type is not currently in a reuse queue, the collection view uses the provided information to create a new cell object automatically.

If you previously registered a class or nib file with the same reuse identifier, the class you specify in the `cellClass` parameter replaces the old entry. You may specify `nil` for `cellClass` if you want to unregister the class from the specified reuse identifier.

## See Also

### Creating cells

struct CellRegistration

A registration for the collection view’s cells.

func dequeueConfiguredReusableCell&lt;Cell, Item>(using: UICollectionView.CellRegistration&lt;Cell, Item>, for: IndexPath, item: Item?) -> Cell

Dequeues a configured reusable cell object.

func register(UINib?, forCellWithReuseIdentifier: String)

Registers a nib file for use in creating new collection view cells.

func dequeueReusableCell(withReuseIdentifier: String, for: IndexPath) -> UICollectionViewCell

Dequeues a reusable cell object located by its identifier.

