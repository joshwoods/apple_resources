

- UIKit
- UISwitch
-  setOn(\_:animated:) 

Instance Method

# setOn(\_:animated:)

Sets the state of the switch to the on or off position, optionally animating the transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setOn(
    _ on: Bool,
    animated: Bool
)
```

## Parameters 

`on`  

true if the switch should be turned to the on position; false if it should be turned to the off position. If the switch is already in the designated position, nothing happens.

`animated`  

true to animate the “flipping” of the switch; otherwise false.

## Discussion

Setting the switch to either position doesn’t result in an action message being sent.

## See Also

### Setting the on/off state

var isOn: Bool

A Boolean value that determines whether the switch is in the on or off position.

