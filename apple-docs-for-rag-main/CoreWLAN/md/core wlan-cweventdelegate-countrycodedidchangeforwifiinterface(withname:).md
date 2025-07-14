

- Core WLAN
- CWEventDelegate
-  countryCodeDidChangeForWiFiInterface(withName:) 

Instance Method

# countryCodeDidChangeForWiFiInterface(withName:)

Tells the delegate that the currently adopted country code has changed.

Mac Catalyst 13.0+macOS 10.6+

``` source
optional func countryCodeDidChangeForWiFiInterface(withName interfaceName: String)
```

## Parameters 

`interfaceName`  

The name of the Wi-Fi interface on which the country code changed.

## Discussion

Register for country code change notifications by sending the startMonitoringEvent(with:) message to a Wi-Fi client object with the CWEventType.countryCodeDidChange event type.

Use the Wi-Fi interface’s countryCode() method to query the currently adopted country code.

## See Also

### Instance Methods

func bssidDidChangeForWiFiInterface(withName: String)

Tells the delegate that the current BSSID has changed.

func clientConnectionInterrupted()

Tells the delegate that the connection to the Wi-Fi subsystem is temporarily interrupted.

func clientConnectionInvalidated()

Tells the delegate that the connection to the Wi-Fi subsystem is permanently invalidated.

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

