

- WatchKit
- WKAccessibilityImageRegion
-  label 

Instance Property

# label

A succinct label that succinctly identifies the purpose of the image region.

watchOS 2.0+

``` source
var label: String { get set }
```

## Discussion

The label should be a very short, localized string that identifies the purpose of the region, but does not necessarily convey the imagery displayed in that region.

## See Also

### Getting the Region Attributes

var frame: CGRect

A portion of the parent image, in the image’s coordinate system.

