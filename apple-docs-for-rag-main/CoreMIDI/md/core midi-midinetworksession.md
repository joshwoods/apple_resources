

- Core MIDI
-  MIDINetworkSession 

Class

# MIDINetworkSession

An object that represents a pairing of a source and destination.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class MIDINetworkSession
```

## Overview

A session can have any number of connections. The system broadcasts output to all connections, and merges input from multiple connections.

## Topics

### Configuring a Session

class func `default`() -> MIDINetworkSession

Returns the default singleton session.

var isEnabled: Bool

A Boolean value that determines whether the session is enabled.

var connectionPolicy: MIDINetworkConnectionPolicy

The policy that determines who can connect to this session.

### Inspecting a Sessions

var localName: String

The name of this session’s entity.

var networkName: String

The name with which this session advertises itself over Bonjour.

var networkPort: Int

The session’s UDP port.

func sourceEndpoint() -> MIDIEndpointRef

Returns the session’s source endpoint.

func destinationEndpoint() -> MIDIEndpointRef

Returns the session’s destination endpoint.

### Managing Connections

func connections() -> Set&lt;MIDINetworkConnection>

Returns the session’s set of MIDI network connections.

func addConnection(MIDINetworkConnection) -> Bool

Adds a new connection to this session.

func removeConnection(MIDINetworkConnection) -> Bool

Removes a connection from this session.

### Managing Contacts

func contacts() -> Set&lt;MIDINetworkHost>

Returns the array of network hosts.

func addContact(MIDINetworkHost) -> Bool

Adds a host as a contact.

func removeContact(MIDINetworkHost) -> Bool

Removes a host as a contact.

let MIDINetworkNotificationContactsDidChange: String

Indicates that the list of contacts changed.

### Observing State Changes

let MIDINetworkNotificationSessionDidChange: String

Indicates that other aspects of the session changed, such as the connection list, connection policy, and so on.

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

## See Also

### Networking

class MIDINetworkHost

An object that represents the host’s network address.

class MIDINetworkConnection

An object that connects a session to a host.

