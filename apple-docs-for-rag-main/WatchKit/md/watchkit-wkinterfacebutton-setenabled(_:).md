

- WatchKit
- WKInterfaceButton
-  setEnabled(\_:) 

Instance Method

# setEnabled(\_:)

Enables or disables the button.

watchOS 2.0+

``` source
func setEnabled(_ enabled: Bool)
```

## Parameters 

`enabled`  

A Boolean value indicating whether the button is enabled or disabled.

## Discussion

When the user taps an enabled button, WatchKit executes the associated action method (if any) in your WatchKit extension code. A disabled button does not respond to taps in its content area.

