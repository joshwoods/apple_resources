

- AppKit
- NSArrayController
-  avoidsEmptySelection 

Instance Property

# avoidsEmptySelection

A Boolean value that indicates whether the receiver requires that the content array attempt to maintain a selection

macOS

``` source
var avoidsEmptySelection: Bool { get set }
```

## Discussion

The default is true. This property is observable using key-value observing.

## See Also

### Selection Attributes

var preservesSelection: Bool

A Boolean value that indicates whether the receiver will attempt to preserve the current selection when the content changes

var alwaysUsesMultipleValuesMarker: Bool

A Boolean value that indicates whether the receiver always returns the multiple values marker when multiple objects are selected

