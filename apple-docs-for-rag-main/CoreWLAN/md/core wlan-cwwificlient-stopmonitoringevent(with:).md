

- Core WLAN
- CWWiFiClient
-  stopMonitoringEvent(with:) 

Instance Method

# stopMonitoringEvent(with:)

Unregister for specific Wi-Fi event notifications.

macOS 10.10+

``` source
func stopMonitoringEvent(with type: CWEventType) throws
```

## Parameters 

`type`  

The type of event notifications to unregister for. See CWEventType for a list of possible values.

## Discussion

Use this method to indicate that the client should no longer send notifications for the given event type.

Note

In order to monitor Wi-Fi events, you must specify the `com.apple.wifi.events` entitlement for your app.

## See Also

### Monitoring Events

func startMonitoringEvent(with: CWEventType) throws

Register for specific Wi-Fi event notifications.

func stopMonitoringAllEvents() throws

Unregister for all Wi-Fi event notifications.

