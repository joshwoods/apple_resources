

- Foundation
- NSNotification
- NSNotification.Name
-  CTRadioAccessTechnologyDidChange Deprecated

Type Property

# CTRadioAccessTechnologyDidChange

The name of the notification indicating that the radio access technology changed for one of the services.

iOS 7.0–12.0DeprecatediPadOS 7.0–12.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
static let CTRadioAccessTechnologyDidChange: NSNotification.Name
```

## Discussion

The notification’s object is an NSString that represents the service identifier of the service whose radio access technology has changed. Use this string as the key in serviceCurrentRadioAccessTechnology to get the value of the new radio access technology for the service.

## See Also

### Core Telephony

static let CTServiceRadioAccessTechnologyDidChange: NSNotification.Name

A notification that posts when radio access technology changes.

