

- Core WLAN
- CWWiFiClient
-  startMonitoringEvent(with:) 

Instance Method

# startMonitoringEvent(with:)

Register for specific Wi-Fi event notifications.

macOS 10.10+

``` source
func startMonitoringEvent(with type: CWEventType) throws
```

## Parameters 

`type`  

The type of event notifications to register for. See CWEventType for a list of possible values.

## Discussion

After registering for notifications, when an event of the given type happens, the client sends an appropriate message to its delegate. See the CWEventDelegate protocol for the complete list of possible messages.

Use the stopMonitoringEvent(with:) method when you want to stop receiving notifications of the given event type. Use stopMonitoringAllEvents() to stop receiving all notifications from a client.

Note

In order to monitor Wi-Fi events, you must specify the `com.apple.wifi.events` entitlement for your app.

## See Also

### Monitoring Events

func stopMonitoringAllEvents() throws

Unregister for all Wi-Fi event notifications.

func stopMonitoringEvent(with: CWEventType) throws

Unregister for specific Wi-Fi event notifications.

