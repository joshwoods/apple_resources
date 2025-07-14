

- Foundation
- NSNotification
- NSNotification.Name
-  CWScanCacheDidUpdate Deprecated

Type Property

# CWScanCacheDidUpdate

macOS 10.7–10.10Deprecated

``` source
static let CWScanCacheDidUpdate: NSNotification.Name
```

Deprecated

Use -\[CWWiFiClient startMonitoringEventWithType:error:\] with the CWEventTypeScanCacheUpdated event type

## Discussion

Posted when new entries are added to the scan cache, or existing entries are updated with more current information. The *object* for this notification is the corresponding BSD interface name. This notification does not contain a *userInfo* dictionary.

## See Also

### Core WLAN

static let CWBSSIDDidChange: NSNotification.NameDeprecated

static let CWCountryCodeDidChange: NSNotification.NameDeprecated

static let CWLinkDidChange: NSNotification.NameDeprecated

static let CWLinkQualityDidChange: NSNotification.NameDeprecated

static let CWModeDidChange: NSNotification.NameDeprecated

static let CWPowerDidChange: NSNotification.NameDeprecated

static let CWSSIDDidChange: NSNotification.NameDeprecated

