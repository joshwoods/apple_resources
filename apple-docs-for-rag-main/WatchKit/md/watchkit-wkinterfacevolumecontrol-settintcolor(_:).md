

- WatchKit
- WKInterfaceVolumeControl
-  setTintColor(\_:) 

Instance Method

# setTintColor(\_:)

Sets the volume control’s tint color.

watchOS 5.0+

``` source
func setTintColor(_ tintColor: UIColor?)
```

## Parameters 

`tintColor`  

The tint color for the volume control. If `nil`, the system uses the app’s tint color.

## Discussion

The system only applies the tint color to the control’s default state (when the crown is not being used to adjust the volume).

