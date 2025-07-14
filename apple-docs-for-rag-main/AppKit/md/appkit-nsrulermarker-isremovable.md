

- AppKit
- NSRulerMarker
-  isRemovable 

Instance Property

# isRemovable

A Boolean that indicates whether the user can remove the receiver from its ruler view.

macOS

``` source
var isRemovable: Bool { get set }
```

## Discussion

true to allow the user to drag the marker image off of the ruler and remove the marker, false to prevent the user from removing the marker.

By default ruler markers are not removable.

## See Also

### Setting movability

var isMovable: Bool

A Boolean that indicates whether the user can move the receiver in its ruler view.

