

- AppKit
- NSProgressIndicator
-  controlTint Deprecated

Instance Property

# controlTint

The progress indicator’s control tint.

macOS 10.0–14.0Deprecated

``` source
@MainActor
var controlTint: NSControlTint { get set }
```

Deprecated

The controlTint property is not respected on 10.15 and later

## Discussion

See NSCell for possible values.

## See Also

### Setting the appearance

var controlSize: NSControl.ControlSize

The size of the progress indicator.

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

