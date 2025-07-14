

- DeviceDiscoveryExtension
- DDDiscoveryExtension
-  stopDiscovery(session:) 

Instance Method

# stopDiscovery(session:)

Ends the extension’s device discovery process.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOSvisionOS

``` source
func stopDiscovery(session: DDDiscoverySession)
```

**Required**

## Parameters 

`session`  

An object that reports discovery events.

## Discussion

The system controls the discovery process using this function by calling it when AVRoutePickerView dismisses. Your extension’s implementation performs any cleanup necessary, such as stopping Bluetooth or Bonjour scanning.

## See Also

### Controlling discovery

func startDiscovery(session: DDDiscoverySession)

Begins the extension’s device discovery process.

**Required**

