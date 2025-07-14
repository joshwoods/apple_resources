

- AppKit
- NSControl
-  sizeThatFits(\_:) 

Instance Method

# sizeThatFits(\_:)

Asks the control to calculate and return the size that best fits the specified size.

macOS 10.10+

``` source
@MainActor
func sizeThatFits(_ size: NSSize) -> NSSize
```

## Parameters 

`size`  

The size for which the control should calculate its best-fitting size.

## Return Value

A new size that fits the receiver’s subviews.

## Discussion

By default, this method returns the intrinsicContentSize of the receiver.

## See Also

### Resizing the Control

var controlSize: NSControl.ControlSize

The size of the control.

enum ControlSize

A constant for specifying a cell’s size.

func sizeToFit()

Resizes the receiver’s frame so that it’s the minimum size needed to contain its cell.

