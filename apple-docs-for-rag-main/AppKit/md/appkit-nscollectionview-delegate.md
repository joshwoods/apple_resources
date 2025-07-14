

- AppKit
- NSCollectionView
-  delegate 

Instance Property

# delegate

The collection view’s delegate object.

macOS 10.5+

``` source
@MainActor
weak var delegate: (any NSCollectionViewDelegate)? { get set }
```

## Discussion

Use the delegate object to manage the selection and highlighting of items, track the addition and removal of items, and manage drag and drop operations. The object you assign to this property must conform to the NSCollectionViewDelegate protocol. The default value of this property is `nil`.

## See Also

### Configuring the Collection View

protocol NSCollectionViewDelegate

A set of methods that you use to manage the behavior of a collection view.

var content: [Any]

An array that provides data for the collection view.

var backgroundView: NSView?

The background view placed behind all items and supplementary views.

var backgroundColors: [NSColor]!

An array containing the collection view’s background colors.

var backgroundViewScrollsWithContent: Bool

A Boolean value that indicates whether the collection view’s background view scrolls with the items and other content.

