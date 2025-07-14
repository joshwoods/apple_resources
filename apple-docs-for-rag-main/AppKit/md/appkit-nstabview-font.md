

- AppKit
- NSTabView
-  font 

Instance Property

# font

The font used for the tab view’s label text.

macOS

``` source
@MainActor
var font: NSFont { get set }
```

## Discussion

The default value of this property is the message font of default size (see messageFont(ofSize:)), which is equivalent to the system font of default size. Tab height is adjusted automatically to accommodate a new font size. If the view allows truncating, tab labels are truncated as needed.

## See Also

### Related Documentation

var allowsTruncatedLabels: Bool

A Boolean value that indicates if the tab view allows truncating for labels that don’t fit on a tab.

