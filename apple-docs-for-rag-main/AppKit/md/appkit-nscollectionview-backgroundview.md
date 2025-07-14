

- AppKit
- NSCollectionView
-  backgroundView 

Instance Property

# backgroundView

The background view placed behind all items and supplementary views.

macOS 10.11+

``` source
@MainActor
var backgroundView: NSView? { get set }
```

## Discussion

The view you assign to this property is positioned underneath all other content and sized automatically to match the enclosing clip view’s frame. The view itself does not scroll with the rest of the collection view content. The view’s layer redraw policy is also changed to NSView.LayerContentsRedrawPolicy.never.

In macOS 10.12 and later, a collection view that sets both backgroundView and backgroundColors shows `backgroundColors[0]` through all areas that are not opaquely covered by the backgroundView.

## See Also

### Configuring the Collection View

var delegate: (any NSCollectionViewDelegate)?

The collection view’s delegate object.

protocol NSCollectionViewDelegate

A set of methods that you use to manage the behavior of a collection view.

var content: [Any]

An array that provides data for the collection view.

var backgroundColors: [NSColor]!

An array containing the collection view’s background colors.

var backgroundViewScrollsWithContent: Bool

A Boolean value that indicates whether the collection view’s background view scrolls with the items and other content.

