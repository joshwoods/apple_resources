

- Objective-C Runtime
- NSObject
-  setupPanel(\_:deviceCouldBeTarget:) 

Instance Method

# setupPanel(\_:deviceCouldBeTarget:)

Allows the delegate to determine if device can be used as a target.

macOS

``` source
func setupPanel(
    _ aPanel: DRSetupPanel!,
    deviceCouldBeTarget device: DRDevice!
) -> Bool
```

## Parameters 

`aPanel`  

The panel.

`device`  

The candidate device.

## Return Value

`YES` if the device is acceptable, `NO` if not.

## Discussion

This method is used to limit the menu to only those devices that you want to appear. For example, a DVD burning application might use this to limit the menu to only devices that are capable of writing DVD-Rs.

