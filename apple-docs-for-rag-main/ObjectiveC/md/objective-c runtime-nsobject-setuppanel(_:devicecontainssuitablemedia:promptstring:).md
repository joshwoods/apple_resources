

- Objective-C Runtime
- NSObject
-  setupPanel(\_:deviceContainsSuitableMedia:promptString:) 

Instance Method

# setupPanel(\_:deviceContainsSuitableMedia:promptString:)

This delegate method allows the delegate to determine if the media inserted in the device is suitable for whatever operation is to be performed.

macOS

``` source
func setupPanel(
    _ aPanel: DRSetupPanel!,
    deviceContainsSuitableMedia device: DRDevice!,
    promptString prompt: AutoreleasingUnsafeMutablePointer!
) -> Bool
```

## Parameters 

`aPanel`  

The panel.

`device`  

The device that contains the media being asked about.

`prompt`  

A pointer to storage for an NSString. Pass back an NSString object describing the media state.

## Return Value

Return `NO` to disable the default button.

