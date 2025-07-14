

- Objective-C Runtime
- NSObject
-  setupPanel(\_:determineBestDeviceOfA:orB:) 

Instance Method

# setupPanel(\_:determineBestDeviceOfA:orB:)

Allows the delegate to specify which device is its preferred.

macOS

``` source
func setupPanel(
    _ aPanel: DRSetupPanel!,
    determineBestDeviceOfA deviceA: DRDevice!,
    orB device: DRDevice!
) -> DRDevice!
```

## Parameters 

`aPanel`  

The panel.

`deviceA`  

A candidate device. May be nil.

`device`  

A candidate device. May be nil.

## Return Value

One of the two device objects passed in.

## Discussion

When the setup panel is first displayed and again, each time a new device appears, the setup panel will ask the delegate to compare two devices to determine which is most suitable for their content to burn.

