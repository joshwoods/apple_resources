

- Foundation
- NSNotification
- NSNotification.Name
-  CTServiceRadioAccessTechnologyDidChange 

Type Property

# CTServiceRadioAccessTechnologyDidChange

A notification that posts when radio access technology changes.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
static let CTServiceRadioAccessTechnologyDidChange: NSNotification.Name
```

## Discussion

The notification’s `object` is a string that represents the identifier of the service with changes to its radio access technology. Use this identifier as the key in serviceCurrentRadioAccessTechnology to get the value of the new radio access technology for the service.

## See Also

### Core Telephony

static let CTRadioAccessTechnologyDidChange: NSNotification.Name

The name of the notification indicating that the radio access technology changed for one of the services.

Deprecated

