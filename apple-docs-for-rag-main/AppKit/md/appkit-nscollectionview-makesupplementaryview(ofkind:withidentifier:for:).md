

- AppKit
- NSCollectionView
-  makeSupplementaryView(ofKind:withIdentifier:for:) 

Instance Method

# makeSupplementaryView(ofKind:withIdentifier:for:)

Creates or returns a reusable supplementary view of the specified type.

macOS 10.11+

``` source
@MainActor
func makeSupplementaryView(
    ofKind elementKind: NSCollectionView.SupplementaryElementKind,
    withIdentifier identifier: NSUserInterfaceItemIdentifier,
    for indexPath: IndexPath
) -> NSView
```

## Parameters 

`elementKind`  

The kind of supplementary view to create. This value is defined by the layout object. This parameter must not be an empty string or `nil`.

`identifier`  

The reuse identifier for the specified item. This is the identifier you specified when registering the supplementary view. This parameter must not be `nil`.

`indexPath`  

The index path specifying the location of the supplementary view. The data source object receives this information in its collectionView(_:viewForSupplementaryElementOfKind:at:) method and you should just pass it along.

## Return Value

A view that adopts the NSCollectionViewElement protocol.

## Discussion

This method looks for a recycled supplementary view of the specified type and returns it if one exists. If one does not exist, it creates it using one of the following techniques:

- If you used the register(_:forSupplementaryViewOfKind:withIdentifier:) method to register a class for the identifier, this method instantiates your view class and returns it.

- If you used the register(_:forSupplementaryViewOfKind:withIdentifier:) method to register a nib file for the identifier, this method loads the view from the nib file and returns it.

## See Also

### Creating Collection View Items

func makeItem(withIdentifier: NSUserInterfaceItemIdentifier, for: IndexPath) -> NSCollectionViewItem

Creates or returns a reusable item object of the specified type.

func register(AnyClass?, forItemWithIdentifier: NSUserInterfaceItemIdentifier)

Registers a class to use when creating new items in the collection view.

func register(NSNib?, forItemWithIdentifier: NSUserInterfaceItemIdentifier)

Registers a nib file to use when creating items in the collection view.

func register(AnyClass?, forSupplementaryViewOfKind: NSCollectionView.SupplementaryElementKind, withIdentifier: NSUserInterfaceItemIdentifier)

Registers a class to use when creating new supplementary views in the collection view.

func register(NSNib?, forSupplementaryViewOfKind: NSCollectionView.SupplementaryElementKind, withIdentifier: NSUserInterfaceItemIdentifier)

Registers a nib file to use when creating supplementary views in the collection view.

typealias SupplementaryElementKind

struct NSUserInterfaceItemIdentifier

