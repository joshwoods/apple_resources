

- AppKit
- NSArrayController
-  alwaysUsesMultipleValuesMarker 

Instance Property

# alwaysUsesMultipleValuesMarker

A Boolean value that indicates whether the receiver always returns the multiple values marker when multiple objects are selected

macOS

``` source
var alwaysUsesMultipleValuesMarker: Bool { get set }
```

## Discussion

The default is false. Setting to true can increase performance if your application doesn’t allow editing multiple values. This property is observable using key-value observing.

## See Also

### Selection Attributes

var avoidsEmptySelection: Bool

A Boolean value that indicates whether the receiver requires that the content array attempt to maintain a selection

var preservesSelection: Bool

A Boolean value that indicates whether the receiver will attempt to preserve the current selection when the content changes

