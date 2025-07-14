

- SMS and Call Reporting
-  CallLookupExtensionStatus 

Enumeration

# CallLookupExtensionStatus

Returns a value with the current state of the app extension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
enum CallLookupExtensionStatus
```

## Topics

### Checking the state of the app extension

case disabled

The Live Caller ID Lookup app extension is in a disabled state.

case enabled

The Live Caller ID Lookup app extension is in an enabled state.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Live Caller ID Lookup

Understanding how Live Caller ID Lookup preserves privacy

Use Live Caller ID Lookup to protect user privacy by hiding the client’s IP address, using anonymous authentication, and hiding the incoming phone number.

Formatting data for blocking and identity information

Set up your PIR payload for call blocking and identity information.

Setting up the HTTP endpoints for Live Caller ID Lookup

Connect the on-device system to your server.

Getting up-to-date calling and blocking information for your app

Implement the Live Caller ID Lookup app extension to provide call-blocking and identity services.

protocol LiveCallerIDLookupProtocol

Information the system uses to query the app extension for context.

protocol LiveCallerIDLookupExtensionConfiguration

An object that allows the system to query the app extension.

struct LiveCallerIDLookupExtensionContext

The information the system uses for configuration.

class LiveCallerIDLookupManager

The entry point that provides access to a collection of functions that help manage the state of the Live Caller ID Lookup app extension.

