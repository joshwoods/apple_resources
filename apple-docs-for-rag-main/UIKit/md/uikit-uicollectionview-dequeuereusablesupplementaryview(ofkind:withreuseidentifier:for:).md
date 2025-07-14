

- UIKit
- UICollectionView
-  dequeueReusableSupplementaryView(ofKind:withReuseIdentifier:for:) 

Instance Method

# dequeueReusableSupplementaryView(ofKind:withReuseIdentifier:for:)

Dequeues a reusable supplementary view located by its identifier and kind.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dequeueReusableSupplementaryView(
    ofKind elementKind: String,
    withReuseIdentifier identifier: String,
    for indexPath: IndexPath
) -> UICollectionReusableView
```

## Parameters 

`elementKind`  

The kind of supplementary view to retrieve. This value is defined by the layout object. This parameter must not be `nil`.

`identifier`  

The reuse identifier for the specified view. This parameter must not be `nil`.

`indexPath`  

The index path specifying the location of the supplementary view in the collection view. The data source receives this information when it’s asked for the view and should just pass it along. This method uses the information to perform additional configuration based on the view’s position in the collection view.

## Return Value

A valid UICollectionReusableView object.

## Discussion

Call this method from your data source object when asked to provide a new supplementary view for the collection view. This method dequeues an existing view if one is available or creates a new one based on the class or nib file you previously registered.

Important

You must register a class or nib file using the register(_:forSupplementaryViewOfKind:withReuseIdentifier:) or register(_:forSupplementaryViewOfKind:withReuseIdentifier:) method before calling this method. You can also register a set of default supplementary views with the layout object using the register(_:forDecorationViewOfKind:) or register(_:forDecorationViewOfKind:) method.

If you registered a class for the specified `identifier` and a new cell must be created, this method initializes the cell by calling its init(frame:) method. For nib-based cells, this method loads the cell object from the provided nib file. If an existing cell was available for reuse, this method calls the cell’s prepareForReuse() method instead.

## See Also

### Creating headers and footers

struct SupplementaryRegistration

A registration for the collection view’s supplementary views.

func dequeueConfiguredReusableSupplementary&lt;Supplementary>(using: UICollectionView.SupplementaryRegistration&lt;Supplementary>, for: IndexPath) -> Supplementary

Dequeues a configured reusable supplementary view object.

func register(AnyClass?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a class for use in creating supplementary views for the collection view.

func register(UINib?, forSupplementaryViewOfKind: String, withReuseIdentifier: String)

Registers a nib file for use in creating supplementary views for the collection view.

