

- AppKit
- NSColorPanel
-  setAction(\_:) 

Instance Method

# setAction(\_:)

Sets the color panel’s action message.

macOS

``` source
@MainActor
func setAction(_ selector: Selector?)
```

## Parameters 

`selector`  

The action message.

## Discussion

When you select a color in the color panel `NSColorPanel` sends its action to its target, provided that neither the action nor the target is `nil`. The action is `NULL` by default.

## See Also

### Configuring the Color Panel

var accessoryView: NSView?

The accessory view.

var isContinuous: Bool

A Boolean value indicating whether the receiver continuously sends the action message to the target.

func setTarget(Any?)

Sets the target of the receiver.

var showsAlpha: Bool

A Boolean value that indicates whether the receiver shows alpha values and an opacity slider.

