

- WatchKit
- WKInterfaceSlider
-  setEnabled(\_:) 

Instance Method

# setEnabled(\_:)

Enables or disables the slider.

watchOS 2.0+

``` source
func setEnabled(_ enabled: Bool)
```

## Parameters 

`enabled`  

A Boolean value indicating whether the slider is enabled or disabled.

## Discussion

A disabled slider does not respond to taps in its up and down buttons. When the user taps an enabled slider, WatchKit updates the slider value and executes the associated action method (if any) in your WatchKit extension.

