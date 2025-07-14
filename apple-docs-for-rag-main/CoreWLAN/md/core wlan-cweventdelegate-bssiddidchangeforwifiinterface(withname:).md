

- Core WLAN
- CWEventDelegate
-  bssidDidChangeForWiFiInterface(withName:) 

Instance Method

# bssidDidChangeForWiFiInterface(withName:)

Tells the delegate that the current BSSID has changed.

Mac Catalyst 13.0+macOS 10.6+

``` source
optional func bssidDidChangeForWiFiInterface(withName interfaceName: String)
```

## Parameters 

`interfaceName`  

The name of the Wi-Fi interface on which the BSSID changed.

## Discussion

Register for BSSID change notifications by sending the startMonitoringEvent(with:) message to a Wi-Fi client object with the CWEventType.bssidDidChange event type.

Use the Wi-Fi interface’s bssid() method to query the current BSSID.

## See Also

### Instance Methods

func clientConnectionInterrupted()

Tells the delegate that the connection to the Wi-Fi subsystem is temporarily interrupted.

func clientConnectionInvalidated()

Tells the delegate that the connection to the Wi-Fi subsystem is permanently invalidated.

func countryCodeDidChangeForWiFiInterface(withName: String)

Tells the delegate that the currently adopted country code has changed.

func linkDidChangeForWiFiInterface(withName: String)

Tells the delegate that the Wi-Fi link state changed.

func linkQualityDidChangeForWiFiInterface(withName: String, rssi: Int, transmitRate: Double)

Tells the delegate that the link quality has changed.

func modeDidChangeForWiFiInterface(withName: String)

Tells the delegate that the operating mode has changed.

func powerStateDidChangeForWiFiInterface(withName: String)

Tells the delegate that the Wi-Fi power state changed.

func scanCacheUpdatedForWiFiInterface(withName: String)

Tells the delegate that the Wi-Fi interface’s scan cache has been updated with new results.

func ssidDidChangeForWiFiInterface(withName: String)

Tells the delegate that the current SSID has changed.

