

- UIKit
- UISwitch
-  isOn 

Instance Property

# isOn

A Boolean value that determines whether the switch is in the on or off position.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isOn: Bool { get set }
```

## Discussion

This property allows you to retrieve and set (without animation) a value determining whether the UISwitch object is on or off.

## See Also

### Setting the on/off state

func setOn(Bool, animated: Bool)

Sets the state of the switch to the on or off position, optionally animating the transition.

