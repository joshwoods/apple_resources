

- AppKit
- NSColorPanel
-  setTarget(\_:) 

Instance Method

# setTarget(\_:)

Sets the target of the receiver.

macOS

``` source
@MainActor
func setTarget(_ target: Any?)
```

## Parameters 

`target`  

The target of the receiver. When you select a color in the color panel `NSColorPanel` sends its action to its target, provided that neither the action nor the target is `nil`. The target is `nil` by default.

## See Also

### Related Documentation

class NSColorPanel

A standard user interface for selecting color in an app.

### Configuring the Color Panel

var accessoryView: NSView?

The accessory view.

var isContinuous: Bool

A Boolean value indicating whether the receiver continuously sends the action message to the target.

func setAction(Selector?)

Sets the color panel’s action message.

var showsAlpha: Bool

A Boolean value that indicates whether the receiver shows alpha values and an opacity slider.

