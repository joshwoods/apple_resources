

- AppKit
- NSProgressIndicator
-  isIndeterminate 

Instance Property

# isIndeterminate

A Boolean that indicates whether the progress indicator is indeterminate.

macOS

``` source
@MainActor
var isIndeterminate: Bool { get set }
```

## Discussion

A determinate indicator displays how much of the task has been completed. An indeterminate indicator shows simply that the app is busy.

When the value of this property is true, the progress indicator is indeterminate; otherwise, it is determinate.

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

var style: NSProgressIndicator.Style

The style of the progress indicator (bar or spinning).

func sizeToFit()

This action method resizes the progress indicator to an appropriate size depending on the value of style.

var isDisplayedWhenStopped: Bool

A Boolean that indicates whether the progress indicator hides itself when it isn’t animating.

