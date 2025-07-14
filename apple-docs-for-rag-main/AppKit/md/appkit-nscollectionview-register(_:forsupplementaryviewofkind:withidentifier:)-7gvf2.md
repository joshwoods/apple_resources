

- AppKit
- NSCollectionView
-  register(\_:forSupplementaryViewOfKind:withIdentifier:) 

Instance Method

# register(\_:forSupplementaryViewOfKind:withIdentifier:)

Registers a nib file to use when creating supplementary views in the collection view.

macOS 10.11+

``` source
@MainActor
func register(
    _ nib: NSNib?,
    forSupplementaryViewOfKind kind: NSCollectionView.SupplementaryElementKind,
    withIdentifier identifier: NSUserInterfaceItemIdentifier
)
```

## Parameters 

`nib`  

The nib object containing the supplementary view’s definition. The nib file must contain exactly one NSView object at the top level and that view must conform to the NSCollectionViewElement protocol. Specify `nil` to unregister a previously registered class or nib file.

`kind`  

The kind of the supplementary view. Layout objects define the kinds of supplementary views they support and are responsible for providing appropriate strings that you can pass for this parameter. This parameter must not be an empty string or `nil`.

`identifier`  

The string that identifies the type of supplementary view. You use this string later when requesting new views and it must be unique among the other registered item and view classes of this collection view. This parameter must not be an empty string or `nil`.

## Discussion

Use this method to register nib files containing prototype supplementary views in your collection view. When you request a view using the makeSupplementaryView(ofKind:withIdentifier:for:) method, the collection view recycles an existing view with the same `identifier` and `kind` values or creates a new one by loading the contents of your nib file.

The layout object is responsible for defining the kind of supplementary views it supports and how those views are used. For example, the flow layout (NSCollectionViewFlowLayout class) lets you specify supplementary views to act as headers and footers for each section.

Typically, you register your supplementary views when initializing your collection view interface. Although you can register new views at any time, you must not call the makeSupplementaryView(ofKind:withIdentifier:for:) method until after you register the corresponding view.

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

typealias SupplementaryElementKind

struct NSUserInterfaceItemIdentifier

