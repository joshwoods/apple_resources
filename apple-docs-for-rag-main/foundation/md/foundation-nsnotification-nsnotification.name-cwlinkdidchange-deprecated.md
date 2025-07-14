

- Foundation
- NSNotification
- NSNotification.Name
-  CWLinkDidChange Deprecated

Type Property

# CWLinkDidChange

macOS 10.6–10.10Deprecated

``` source
static let CWLinkDidChange: NSNotification.Name
```

Deprecated

Use -\[CWWiFiClient startMonitoringEventWithType:error:\] with the CWEventTypeLinkDidChange event type

## Discussion

Posted when the link state of any WLAN interface changes. The *object* for this notification is the corresponding BSD interface name. This notification does not contain a *userInfo* dictionary.

## See Also

### Core WLAN

static let CWBSSIDDidChange: NSNotification.NameDeprecated

static let CWCountryCodeDidChange: NSNotification.NameDeprecated

static let CWLinkQualityDidChange: NSNotification.NameDeprecated

static let CWModeDidChange: NSNotification.NameDeprecated

static let CWPowerDidChange: NSNotification.NameDeprecated

static let CWSSIDDidChange: NSNotification.NameDeprecated

static let CWScanCacheDidUpdate: NSNotification.NameDeprecated

