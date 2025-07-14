

- WatchKit
- WKInterfaceSwitch
-  setOn(\_:) 

Instance Method

# setOn(\_:)

Sets the state of the switch to the specified value.

watchOS 2.0+

``` source
func setOn(_ on: Bool)
```

## Parameters 

`on`  

A Boolean value indicating whether the switch should be set to the On or Off state. Specify true to set the switch to the On state.

## Discussion

Use this method to set the value of a switch. If you want to know the value of a switch, use a local variable to track that information.

## See Also

### Configuring the Switch

func setColor(UIColor?)

Changes the tint color of the switch when it is on.

