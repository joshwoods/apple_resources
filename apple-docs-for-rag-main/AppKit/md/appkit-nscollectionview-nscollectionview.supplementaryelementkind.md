

- AppKit
- NSCollectionView
-  NSCollectionView.SupplementaryElementKind 

Type Alias

# NSCollectionView.SupplementaryElementKind

macOS

``` source
typealias SupplementaryElementKind = String
```

## See Also

### Creating Collection View Items

func makeItem(withIdentifier: NSUserInterfaceItemIdentifier, for: IndexPath) -> NSCollectionViewItem

Creates or returns a reusable item object of the specified type.

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

struct NSUserInterfaceItemIdentifier

