

- Foundation
- NSNotification
- NSNotification.Name
-  CWBSSIDDidChange Deprecated

Type Property

# CWBSSIDDidChange

macOS 10.6–10.10Deprecated

``` source
static let CWBSSIDDidChange: NSNotification.Name
```

Deprecated

Use -\[CWWiFiClient startMonitoringEventWithType:error:\] with the CWEventTypeBSSIDDidChange event type

## Discussion

Posted when the BSSID of any WLAN interface changes. The *object* for this notification is the corresponding BSD interface name. This notification does not contain a *userInfo* dictionary.

## See Also

### Core WLAN

static let CWCountryCodeDidChange: NSNotification.NameDeprecated

static let CWLinkDidChange: NSNotification.NameDeprecated

static let CWLinkQualityDidChange: NSNotification.NameDeprecated

static let CWModeDidChange: NSNotification.NameDeprecated

static let CWPowerDidChange: NSNotification.NameDeprecated

static let CWSSIDDidChange: NSNotification.NameDeprecated

static let CWScanCacheDidUpdate: NSNotification.NameDeprecated

