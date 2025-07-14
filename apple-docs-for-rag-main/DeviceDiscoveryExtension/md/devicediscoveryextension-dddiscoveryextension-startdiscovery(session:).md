

- DeviceDiscoveryExtension
- DDDiscoveryExtension
-  startDiscovery(session:) 

Instance Method

# startDiscovery(session:)

Begins the extension’s device discovery process.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOSvisionOS

``` source
func startDiscovery(session: DDDiscoverySession)
```

**Required**

## Parameters 

`session`  

An object that reports discovery events.

## Discussion

The system controls the discovery process using this function by calling it when AVRoutePickerView displays. You code your extension to search the local network or paired Bluetooth devices for a third-party device of interest that you want the system to include in the picker.

## See Also

### Controlling discovery

func stopDiscovery(session: DDDiscoverySession)

Ends the extension’s device discovery process.

**Required**

