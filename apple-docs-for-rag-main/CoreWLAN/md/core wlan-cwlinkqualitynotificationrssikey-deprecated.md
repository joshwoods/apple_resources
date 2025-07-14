

- Core WLAN
-  CWLinkQualityNotificationRSSIKey Deprecated

Global Variable

# CWLinkQualityNotificationRSSIKey

macOS 10.6–10.10Deprecated

``` source
let CWLinkQualityNotificationRSSIKey: String
```

Deprecated

Use -\[CWWiFiClient startMonitoringEventWithType:error:\] with the CWEventTypeLinkQualityDidChange event type

## Discussion

NSNumber containing the current RSSI value for the WLAN interface. Found in the *userInfo* dictionary for the *CWLinkQualityChangedNotification*.

## See Also

### Constants

let CWErrorDomain: String

let CWLinkQualityNotificationTransmitRateKey: StringDeprecated

