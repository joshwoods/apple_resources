

- Core WLAN
- CWWiFiClient
-  delegate 

Instance Property

# delegate

An object that provides Wi-Fi event handling.

macOS 10.10+

``` source
weak var delegate: AnyObject? { get set }
```

## Discussion

When a client registers for Wi-Fi events with the startMonitoringEvent(with:) method, the client’s delegate receives messages in response to Wi-Fi events. The delegate should adopt the CWEventDelegate protocol to receive these messages.

