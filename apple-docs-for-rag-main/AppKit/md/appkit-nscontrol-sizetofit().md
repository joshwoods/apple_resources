

- AppKit
- NSControl
-  sizeToFit() 

Instance Method

# sizeToFit()

Resizes the receiver’s frame so that it’s the minimum size needed to contain its cell.

macOS

``` source
@MainActor
func sizeToFit()
```

## Discussion

If you want a multiple-cell custom subclass of `NSControl` to size itself to fit its cells, you must override this method. This method neither redisplays the receiver nor marks it as needing display. You must do this yourself with either thedisplay() or setNeedsDisplay() method.

## See Also

### Related Documentation

func calcSize()

Recomputes any internal sizing information for the receiver, if necessary.

Deprecated

### Resizing the Control

var controlSize: NSControl.ControlSize

The size of the control.

enum ControlSize

A constant for specifying a cell’s size.

func sizeThatFits(NSSize) -> NSSize

Asks the control to calculate and return the size that best fits the specified size.

