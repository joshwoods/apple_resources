

- UIKit
- UIView
-  autoresizesSubviews 

Instance Property

# autoresizesSubviews

A Boolean value that determines whether the receiver automatically resizes its subviews when its bounds change.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var autoresizesSubviews: Bool { get set }
```

## Discussion

When set to true, the receiver adjusts the size of its subviews when its bounds change. The default value is true.

## See Also

### Configuring the resizing behavior

var contentMode: UIView.ContentMode

A flag used to determine how a view lays out its content when its bounds change.

enum ContentMode

Options to specify how a view adjusts its content when its size changes.

func sizeThatFits(CGSize) -> CGSize

Asks the view to calculate and return the size that best fits the specified size.

func sizeToFit()

Resizes and moves the receiver view so it just encloses its subviews.

var autoresizingMask: UIView.AutoresizingMask

An integer bit mask that determines how the receiver resizes itself when its superview’s bounds change.

