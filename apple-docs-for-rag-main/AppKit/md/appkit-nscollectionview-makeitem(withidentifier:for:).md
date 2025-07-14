

- AppKit
- NSCollectionView
-  makeItem(withIdentifier:for:) 

Instance Method

# makeItem(withIdentifier:for:)

Creates or returns a reusable item object of the specified type.

macOS 10.11+

``` source
@MainActor
func makeItem(
    withIdentifier identifier: NSUserInterfaceItemIdentifier,
    for indexPath: IndexPath
) -> NSCollectionViewItem
```

## Parameters 

`identifier`  

The reuse identifier for the specified item. This is the identifier you specified when registering the item. This parameter must not be `nil`.

`indexPath`  

The index path specifying the location of the item. The data source object receives this information in its collectionView(_:itemForRepresentedObjectAt:) method and you should just pass it along.

## Return Value

A valid NSCollectionViewItem object.

## Discussion

This method looks for a recycled item object of the specified type and returns it if one exists. If one does not exist, it creates it using one of the following techniques:

- If you used the register(_:forItemWithIdentifier:) method to register a class for the identifier, this method instantiates your class and returns it.

- If you used the register(_:forItemWithIdentifier:) method to register a nib file for the identifier, this method loads the item from the nib file and returns it.

## See Also

### Creating Collection View Items

func register(AnyClass?, forItemWithIdentifier: NSUserInterfaceItemIdentifier)

Registers a class to use when creating new items in the collection view.

func register(NSNib?, forItemWithIdentifier: NSUserInterfaceItemIdentifier)

Registers a nib file to use when creating items in the collection view.

func makeSupplementaryView(ofKind: NSCollectionView.SupplementaryElementKind, withIdentifier: NSUserInterfaceItemIdentifier, for: IndexPath) -> NSView

Creates or returns a reusable supplementary view of the specified type.

func register(AnyClass?, forSupplementaryViewOfKind: NSCollectionView.SupplementaryElementKind, withIdentifier: NSUserInterfaceItemIdentifier)

Registers a class to use when creating new supplementary views in the collection view.

func register(NSNib?, forSupplementaryViewOfKind: NSCollectionView.SupplementaryElementKind, withIdentifier: NSUserInterfaceItemIdentifier)

Registers a nib file to use when creating supplementary views in the collection view.

typealias SupplementaryElementKind

struct NSUserInterfaceItemIdentifier

