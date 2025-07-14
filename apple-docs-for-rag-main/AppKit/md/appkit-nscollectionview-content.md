

- AppKit
- NSCollectionView
-  content 

Instance Property

# content

An array that provides data for the collection view.

macOS 10.5+

``` source
@MainActor
var content: [Any] { get set }
```

## Discussion

The content object manages the data in the collection view. Use this object to specify an array of items directly. This property is observable using key-value observing. The collection view also exposes a `content` binding value so that you can specify the array of items using an ArrayController object in Interface Builder.

To specify the data for your collection view, assign a value to this property or to the dataSource property, but not both. If you specify a value for the dataSource property, the collection view ignores the value in this property.

## See Also

### Configuring the Collection View

var delegate: (any NSCollectionViewDelegate)?

The collection view’s delegate object.

protocol NSCollectionViewDelegate

A set of methods that you use to manage the behavior of a collection view.

var backgroundView: NSView?

The background view placed behind all items and supplementary views.

var backgroundColors: [NSColor]!

An array containing the collection view’s background colors.

var backgroundViewScrollsWithContent: Bool

A Boolean value that indicates whether the collection view’s background view scrolls with the items and other content.

