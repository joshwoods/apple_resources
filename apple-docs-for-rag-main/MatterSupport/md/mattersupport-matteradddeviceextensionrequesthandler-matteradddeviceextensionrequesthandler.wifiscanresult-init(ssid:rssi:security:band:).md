

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
- MatterAddDeviceExtensionRequestHandler.WiFiScanResult
-  init(ssid:rssi:security:band:) 

Initializer

# init(ssid:rssi:security:band:)

Creates a new instance of the request handler.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
init(
    ssid: Data,
    rssi: Int8,
    security: MTRNetworkCommissioningWiFiSecurity,
    band: MTRNetworkCommissioningWiFiBand
)
```

## Parameters 

`ssid`  

The SSID of the Wi-Fi network.

`rssi`  

The device-observed RSSI of the network.

`security`  

The security method used to secure the Wi-Fi network.

`band`  

The band for the Wi-Fi network.

