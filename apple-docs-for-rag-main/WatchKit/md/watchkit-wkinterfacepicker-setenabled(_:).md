

- WatchKit
- WKInterfacePicker
-  setEnabled(\_:) 

Instance Method

# setEnabled(\_:)

Enables or disables the picker.

watchOS 2.0+

``` source
func setEnabled(_ enabled: Bool)
```

## Parameters 

`enabled`  

A Boolean value indicating whether the picker is enabled or disabled.

## Discussion

A disabled picker does not respond to taps in its content area and cannot receive focus. When the user selects an item in an enabled picker, WatchKit executes the associated action method (if any) in your WatchKit extension code.

