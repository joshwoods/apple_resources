

- Core WLAN
- CWWiFiClient
-  stopMonitoringAllEvents() 

Instance Method

# stopMonitoringAllEvents()

Unregister for all Wi-Fi event notifications.

macOS 10.10+

``` source
func stopMonitoringAllEvents() throws
```

## Discussion

Use this method when you no longer want to receive any Wi-Fi notifications from the client.

Note

In order to monitor Wi-Fi events, you must specify the `com.apple.wifi.events` entitlement for your app.

## See Also

### Monitoring Events

func startMonitoringEvent(with: CWEventType) throws

Register for specific Wi-Fi event notifications.

func stopMonitoringEvent(with: CWEventType) throws

Unregister for specific Wi-Fi event notifications.

