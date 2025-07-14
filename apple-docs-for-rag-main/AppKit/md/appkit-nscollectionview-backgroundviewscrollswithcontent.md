

- AppKit
- NSCollectionView
-  backgroundViewScrollsWithContent 

Instance Property

# backgroundViewScrollsWithContent

A Boolean value that indicates whether the collection view’s background view scrolls with the items and other content.

macOS 10.12+

``` source
@MainActor
var backgroundViewScrollsWithContent: Bool { get set }
```

## Discussion

The default value of this property is false, which means that backgroundView (if it exists) fills the collection view’s visible area and remains stationary when the collection view’s content is scrolled. When the value of this property is true, backgroundView matches the collection view’s frame and scrolls with the collection view’s items and other content.

Changing the value of this property also changes the background view’s parent. When backgroundView floats behind the scrolling content, it is a sibling of the collection view’s clip view. When it scrolls with the collection view’s content, it is a subview of the collection view.

## See Also

### Configuring the Collection View

var delegate: (any NSCollectionViewDelegate)?

The collection view’s delegate object.

protocol NSCollectionViewDelegate

A set of methods that you use to manage the behavior of a collection view.

var content: [Any]

An array that provides data for the collection view.

var backgroundView: NSView?

The background view placed behind all items and supplementary views.

var backgroundColors: [NSColor]!

An array containing the collection view’s background colors.

