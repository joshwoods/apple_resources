

- Core WLAN
-  CWLinkQualityNotificationTransmitRateKey Deprecated

Global Variable

# CWLinkQualityNotificationTransmitRateKey

macOS 10.6–10.10Deprecated

``` source
let CWLinkQualityNotificationTransmitRateKey: String
```

Deprecated

Use -\[CWWiFiClient startMonitoringEventWithType:error:\] with the CWEventTypeLinkQualityDidChange event type

## Discussion

NSNumber containing the current transmit rate value for the WLAN interface. Found in the *userInfo* dictionary for the *CWLinkQualityChangedNotification*.

## See Also

### Constants

let CWErrorDomain: String

let CWLinkQualityNotificationRSSIKey: StringDeprecated

