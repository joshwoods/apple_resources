

- AppKit
- NSArrayController
-  preservesSelection 

Instance Property

# preservesSelection

A Boolean value that indicates whether the receiver will attempt to preserve the current selection when the content changes

macOS

``` source
var preservesSelection: Bool { get set }
```

## Discussion

The default is true. This property is observable using key-value observing.

## See Also

### Selection Attributes

var avoidsEmptySelection: Bool

A Boolean value that indicates whether the receiver requires that the content array attempt to maintain a selection

var alwaysUsesMultipleValuesMarker: Bool

A Boolean value that indicates whether the receiver always returns the multiple values marker when multiple objects are selected

