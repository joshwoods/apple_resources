

- Objective-C Runtime
- NSObject
-  setupPanelDeviceSelectionChanged(\_:) 

Instance Method

# setupPanelDeviceSelectionChanged(\_:)

Sent by the default notification center when the device selection in the panel has changed.

macOS

``` source
func setupPanelDeviceSelectionChanged(_ aNotification: Notification!)
```

## Parameters 

`aNotification`  

Notification object. This is always `DRSetupPanelDeviceSelectionChangedNotification`.

## Discussion

You can retrieve the `DRSetupPanel` object in question by sending `NSNotification` object to `aNotification`. The userInfo dictionary contains the single key DRSetupPanelSelectedDeviceKey whose value is the `DRDevice` object that is currently selected.

