

- SMS and Call Reporting
-  Formatting data for blocking and identity information 

Article

# Formatting data for blocking and identity information

Set up your PIR payload for call blocking and identity information.

## Overview

With Live Caller ID Lookup, when a device receives an incoming call, the system reaches out to a third-party service to fetch private information retrieval (PIR) data from your server. You need to format that data so the system can make the following requests:

- A blocking information request

- An identity information request

For more information, see the Swift homomorphic encryption library.

### Block a caller

The blocking information request is a single byte with two defined values:

0  
This value means don’t block the caller.

1  
This value means block the caller.

### Identify caller information

The identity request displays caller information on the device. This information is a serialized protocol buffer message of type `CallIdentity`. The following example shows the response formatting for an identity request:

```
```

## See Also

### Live Caller ID Lookup

Understanding how Live Caller ID Lookup preserves privacy

Use Live Caller ID Lookup to protect user privacy by hiding the client’s IP address, using anonymous authentication, and hiding the incoming phone number.

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

enum CallLookupExtensionStatus

Returns a value with the current state of the app extension.

class LiveCallerIDLookupManager

The entry point that provides access to a collection of functions that help manage the state of the Live Caller ID Lookup app extension.

