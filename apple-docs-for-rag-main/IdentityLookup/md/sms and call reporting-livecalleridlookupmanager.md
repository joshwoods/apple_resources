

- SMS and Call Reporting
-  LiveCallerIDLookupManager 

Class

# LiveCallerIDLookupManager

The entry point that provides access to a collection of functions that help manage the state of the Live Caller ID Lookup app extension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
class LiveCallerIDLookupManager
```

## Mentioned in 

Getting up-to-date calling and blocking information for your app

## Overview

You can use the provided functions to check whether your app extension is in an enabled state, open Settings to enable the extension, and manage refreshing your server data.

## Topics

### Checking status and fetching data

let extensionPointName: String

The name of the extension point.

func openSettings() async throws

Navigates to Settings so a person can configure the Live Caller ID Lookup app extension.

func refreshPIRParameters(forExtensionWithIdentifier: String) async throws

Communicates with the system to refetch Private Information Retrieval (PIR) parameters from the server.

func reset(forExtensionWithIdentifier: String) async throws

Resets the cache associated with the app extension.

func status(forExtensionWithIdentifier: String) -> CallLookupExtensionStatus

Queries the system to check the status of the app extension.

### Sharing the instance

static let shared: LiveCallerIDLookupManager

The shared Live Caller ID Lookup manager instance for the app.

### Instance Methods

func refreshExtensionContext(forExtensionWithIdentifier: String) async throws

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

enum CallLookupExtensionStatus

Returns a value with the current state of the app extension.

