

- AppKit
- NSProgressIndicator
-  isDisplayedWhenStopped 

Instance Property

# isDisplayedWhenStopped

A Boolean that indicates whether the progress indicator hides itself when it isn’t animating.

macOS

``` source
@MainActor
var isDisplayedWhenStopped: Bool { get set }
```

## Discussion

When the value of this property is false, the progress indicator is hidden when it isn’t animating. The default value of this property is true.

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

var style: NSProgressIndicator.Style

The style of the progress indicator (bar or spinning).

func sizeToFit()

This action method resizes the progress indicator to an appropriate size depending on the value of style.

