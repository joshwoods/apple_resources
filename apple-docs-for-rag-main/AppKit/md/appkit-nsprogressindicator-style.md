

- AppKit
- NSProgressIndicator
-  style 

Instance Property

# style

The style of the progress indicator (bar or spinning).

macOS

``` source
@MainActor
var style: NSProgressIndicator.Style { get set }
```

## Discussion

See NSProgressIndicator.Style for possible values.

## See Also

### Setting the appearance

var controlSize: NSControl.ControlSize

The size of the progress indicator.

var controlTint: NSControlTint

The progress indicator’s control tint.

Deprecated

var isBezeled: Bool

A Boolean that indicates whether the progress indicator’s frame has a three-dimensional bezel.

Deprecated

var isIndeterminate: Bool

A Boolean that indicates whether the progress indicator is indeterminate.

func sizeToFit()

This action method resizes the progress indicator to an appropriate size depending on the value of style.

var isDisplayedWhenStopped: Bool

A Boolean that indicates whether the progress indicator hides itself when it isn’t animating.

