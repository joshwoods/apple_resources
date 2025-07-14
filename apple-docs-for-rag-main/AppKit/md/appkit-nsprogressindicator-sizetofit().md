

- AppKit
- NSProgressIndicator
-  sizeToFit() 

Instance Method

# sizeToFit()

This action method resizes the progress indicator to an appropriate size depending on the value of style.

macOS

``` source
@MainActor
func sizeToFit()
```

## Discussion

Use this after you use style to re-size the progress indicator.

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

var isDisplayedWhenStopped: Bool

A Boolean that indicates whether the progress indicator hides itself when it isn’t animating.

