

- Device Management
- GoogleAccount
-  GoogleAccount.CommunicationServiceRules 

Device Management Profile

# GoogleAccount.CommunicationServiceRules

The communication service handler rules for this account.

iOS 9.3+iPadOS 9.3+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object GoogleAccount.CommunicationServiceRules
```

## Properties

`DefaultServiceHandlers`

GoogleAccount.CommunicationServiceRules.DefaultServiceHandlers

A dictionary that defines which app to use for audio calls from this account.

## Discussion

The rules contain only a `DefaultServiceHandlers` key; its value is a dictionary which contains an `AudioCall` key whose value is a string containing the bundle identifier for the default application that handles audio calls to contacts from this account.

## Topics

### Profiles

object GoogleAccount.CommunicationServiceRules.DefaultServiceHandlers

A dictionary of default service handlers.

