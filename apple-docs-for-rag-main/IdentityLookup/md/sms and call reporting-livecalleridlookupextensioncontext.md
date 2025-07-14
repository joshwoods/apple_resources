

- SMS and Call Reporting
-  LiveCallerIDLookupExtensionContext 

Structure

# LiveCallerIDLookupExtensionContext

The information the system uses for configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
struct LiveCallerIDLookupExtensionContext
```

## Mentioned in 

Getting up-to-date calling and blocking information for your app

## Overview

The extension context allows the system to obtain information from your app.

## Topics

### Initializing the app extension context

init(serviceURL: URL, tokenIssuerURL: URL, userTierToken: Data)

Creates the app extension context.

### Configuring the system

let serviceURL: URL

The endpoint of the service to fetch identity and blocking information.

let tokenIssuerURL: URL

The URL of the Privacy Pass token issuer.

let userTierToken: Data

An HTTP bearer token that authenticates the person using your app.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

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

enum CallLookupExtensionStatus

Returns a value with the current state of the app extension.

class LiveCallerIDLookupManager

The entry point that provides access to a collection of functions that help manage the state of the Live Caller ID Lookup app extension.

