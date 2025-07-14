

- DeviceDiscoveryExtension
- DDDiscoverySession
-  report(\_:) 

Instance Method

# report(\_:)

Reports an event to the system.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
func report(_ inEvent: DDDeviceEvent)
```

## Parameters 

`inEvent`  

The event to report.

## Discussion

The extension updates the system with the discovery status of the device of interest by passing event objects (`DDEvent`) through this function.

