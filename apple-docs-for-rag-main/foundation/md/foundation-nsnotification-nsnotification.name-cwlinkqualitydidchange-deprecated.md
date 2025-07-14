

- Foundation
- NSNotification
- NSNotification.Name
-  CWLinkQualityDidChange Deprecated

Type Property

# CWLinkQualityDidChange

macOS 10.7–10.10Deprecated

``` source
static let CWLinkQualityDidChange: NSNotification.Name
```

Deprecated

Use -\[CWWiFiClient startMonitoringEventWithType:error:\] with the CWEventTypeLinkQualityDidChange event type

## Discussion

Posted when the link quality for any WLAN interface changes. The *object* for this notification is the corresponding BSD interface name. The *userInfo* dictionary for this notification contains the current RSSI and current transmit rate for the given CoreWLAN interface.

## See Also

### Core WLAN

static let CWBSSIDDidChange: NSNotification.NameDeprecated

static let CWCountryCodeDidChange: NSNotification.NameDeprecated

static let CWLinkDidChange: NSNotification.NameDeprecated

static let CWModeDidChange: NSNotification.NameDeprecated

static let CWPowerDidChange: NSNotification.NameDeprecated

static let CWSSIDDidChange: NSNotification.NameDeprecated

static let CWScanCacheDidUpdate: NSNotification.NameDeprecated

