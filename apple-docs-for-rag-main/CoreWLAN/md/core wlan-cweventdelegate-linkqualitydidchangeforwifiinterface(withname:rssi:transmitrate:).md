

- Core WLAN
- CWEventDelegate
-  linkQualityDidChangeForWiFiInterface(withName:rssi:transmitRate:) 

Instance Method

# linkQualityDidChangeForWiFiInterface(withName:rssi:transmitRate:)

Tells the delegate that the link quality has changed.

Mac Catalyst 13.0+macOS 10.6+

``` source
optional func linkQualityDidChangeForWiFiInterface(
    withName interfaceName: String,
    rssi: Int,
    transmitRate: Double
)
```

## Parameters 

`interfaceName`  

The name of the Wi-Fi interface on which the link quality changed.

`rssi`  

The receive signal strength indicator (RSSI) value measured in dBm for the currently associated network.

`transmitRate`  

The transmit rate measured in Mbps for the currently associated network.

## Discussion

Register for link quality change notifications by sending the startMonitoringEvent(with:) message to a Wi-Fi client object with the CWEventType.linkQualityDidChange event type.

Use the Wi-Fi interface’s rssiValue() and transmitRate() methods to query the current RSSI and transmit rate, respectively.

## See Also

### Instance Methods

func bssidDidChangeForWiFiInterface(withName: String)

Tells the delegate that the current BSSID has changed.

func clientConnectionInterrupted()

Tells the delegate that the connection to the Wi-Fi subsystem is temporarily interrupted.

func clientConnectionInvalidated()

Tells the delegate that the connection to the Wi-Fi subsystem is permanently invalidated.

func countryCodeDidChangeForWiFiInterface(withName: String)

Tells the delegate that the currently adopted country code has changed.

func linkDidChangeForWiFiInterface(withName: String)

Tells the delegate that the Wi-Fi link state changed.

func modeDidChangeForWiFiInterface(withName: String)

Tells the delegate that the operating mode has changed.

func powerStateDidChangeForWiFiInterface(withName: String)

Tells the delegate that the Wi-Fi power state changed.

func scanCacheUpdatedForWiFiInterface(withName: String)

Tells the delegate that the Wi-Fi interface’s scan cache has been updated with new results.

func ssidDidChangeForWiFiInterface(withName: String)

Tells the delegate that the current SSID has changed.

