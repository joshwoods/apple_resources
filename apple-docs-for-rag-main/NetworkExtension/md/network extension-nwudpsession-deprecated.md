

- Network Extension
-  NWUDPSession Deprecated

Class

# NWUDPSession

An object to manage a UDP session to a network endpoint.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class NWUDPSession
```

Deprecated

Use the nw_connection_t type from the Network framework instead.

## Overview

Since UDP does not include a handshake with the remote endpoint as part of its protocol, it is up to the client of the UDP session to provide feedback on the viability of the current endpoint. If a session is opened to a hostname, the system will resolve that hostname into potentially several IP addresses. Once the session state is `NWUDPSessionStateReady`, the client should try to write and read datagrams. If there is no response from the remote endpoint, the client can try the next address that was resolved using `tryNextResolvedEndpoint`.

## Topics

### Monitoring the session state

var state: NWUDPSessionState

The current state of the UDP session.

enum NWUDPSessionState

var isViable: Bool

The viability of a UDP session represents whether or not data can be transferred.

### Selecting remote endpoints

var resolvedEndpoint: NWEndpoint?

The currently targeted remote endpoint.

func tryNextResolvedEndpoint()

Mark the current value of resolvedEndpoint as unusable, and try to switch to the next available endpoint.

### Transferring data

func setReadHandler(([Data]?, (any Error)?) -> Void, maxDatagrams: Int)

Set a read handler for datagrams.

func writeDatagram(Data, completionHandler: ((any Error)?) -> Void)

Write a single datagram.

func writeMultipleDatagrams([Data], completionHandler: ((any Error)?) -> Void)

Write multiple datagrams.

var maximumDatagramLength: Int

The maximum size of a datagram to be written currently.

### Canceling the session

func cancel()

Cancel the session.

### Responding to network changes

var hasBetterPath: Bool

If a session has a better path, new session would use a different interface.

init(upgradeFor: NWUDPSession)

This convenience initializer can be used to create a new session based on the original session’s endpoint and parameters.

### Getting session properties

var endpoint: NWEndpoint

The destination endpoint with which this session was created.

var currentPath: NWPath?

The current evaluated path for the session’s resolvedEndpoint property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

