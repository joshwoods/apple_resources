

- AppKit
- NSControl
-  controlSize 

Instance Property

# controlSize

The size of the control.

macOS 10.10+

``` source
@MainActor
var controlSize: NSControl.ControlSize { get set }
```

## See Also

### Resizing the Control

enum ControlSize

A constant for specifying a cell’s size.

func sizeThatFits(NSSize) -> NSSize

Asks the control to calculate and return the size that best fits the specified size.

func sizeToFit()

Resizes the receiver’s frame so that it’s the minimum size needed to contain its cell.

