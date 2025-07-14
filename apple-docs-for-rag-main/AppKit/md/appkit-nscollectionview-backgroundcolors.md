

- AppKit
- NSCollectionView
-  backgroundColors 

Instance Property

# backgroundColors

An array containing the collection view’s background colors.

macOS 10.5+

``` source
@MainActor
var backgroundColors: [NSColor]! { get set }
```

## Discussion

This property contains an array of NSColor objects, representing the colors to use when drawing the background grid. Specifying an empty array or `nil` causes the collection view to use the default colors returned by the controlAlternatingRowBackgroundColors method.

When a background view is specified for the collection view, the colors in this property are ignored.

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

var backgroundViewScrollsWithContent: Bool

A Boolean value that indicates whether the collection view’s background view scrolls with the items and other content.

