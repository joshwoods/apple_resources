

- AppKit
- NSProgressIndicator
-  controlSize 

Instance Property

# controlSize

The size of the progress indicator.

macOS

``` source
@MainActor
var controlSize: NSControl.ControlSize { get set }
```

## Discussion

See NSCell for possible values.

## See Also

### Setting the appearance

var controlTint: NSControlTint

The progress indicator’s control tint.

Deprecated

var isBezeled: Bool

A Boolean that indicates whether the progress indicator’s frame has a three-dimensional bezel.

Deprecated

var isIndeterminate: Bool

A Boolean that indicates whether the progress indicator is indeterminate.

var style: NSProgressIndicator.Style

The style of the progress indicator (bar or spinning).

func sizeToFit()

This action method resizes the progress indicator to an appropriate size depending on the value of style.

var isDisplayedWhenStopped: Bool

A Boolean that indicates whether the progress indicator hides itself when it isn’t animating.

