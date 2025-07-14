

- Media Player
-  MPVolumeSettingsAlertShow() Deprecated

Function

# MPVolumeSettingsAlertShow()

Displays an alert panel for controlling the system volume.

iOS 2.0–11.3DeprecatediPadOS 2.0–11.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func MPVolumeSettingsAlertShow()
```

Deprecated

Use MPVolumeView to present volume controls.

## Discussion

The alert panel displayed by this function floats above the contents of the current window. It contains a slider for adjusting the system volume setting and a Done button so that the user can dismiss the panel. You can also dismiss the panel programmatically using the MPVolumeSettingsAlertHide() function.

## See Also

### Global volume setting methods

func MPVolumeSettingsAlertHide()

Hides the alert panel that controls the system volume.

Deprecated

func MPVolumeSettingsAlertIsVisible() -> Bool

Returns a Boolean value indicating whether the volume alert panel is currently visible.

Deprecated

