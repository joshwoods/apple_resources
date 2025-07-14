

- WatchKit
- WKInterfaceSwitch
-  setEnabled(\_:) 

Instance Method

# setEnabled(\_:)

Enables or disables the switch.

watchOS 2.0+

``` source
func setEnabled(_ enabled: Bool)
```

## Parameters 

`enabled`  

A Boolean value indicating whether the switch is enabled or disabled.

## Discussion

A disabled switch does not respond to taps in its content area. When the user taps an enabled switch, WatchKit executes the associated action method (if any) in your WatchKit extension.

