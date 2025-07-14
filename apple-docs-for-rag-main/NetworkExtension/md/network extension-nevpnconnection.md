

- Network Extension
-  NEVPNConnection 

Class

# NEVPNConnection

An object to start and stop a Personal VPN connection and get its status.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEVPNConnection
```

## Overview

NEVPNConnection objects are not instantiated directly. Instead, each `NEVPNManager` object has an associated NEVPNConnection object as a read-only property.

The NEVPNConnection class provides methods for starting and stopping the VPN programmatically. The other way that the VPN can be started and stopped is through VPN On Demand. See the `onDemandRules` property in NEVPNManager and NEOnDemandRule.

Instances of this class are thread safe.

## Topics

### Controlling the VPN connection

func startVPNTunnel() throws

Start the process of connecting the VPN.

func startVPNTunnel(options: [String : NSObject]?) throws

Start the process of connecting the VPN.

let NEVPNConnectionStartOptionUsername: String

let NEVPNConnectionStartOptionPassword: String

func stopVPNTunnel()

Start the process of disconnecting the VPN.

### Getting VPN connection status

var manager: NEVPNManager

var status: NEVPNStatus

The current status of the VPN connection.

enum NEVPNStatus

The possible states of a VPN connection.

var connectedDate: Date?

The date and time when the connection status changed to `NEVPNStatusConnected`.

### Notifications

static let NEVPNStatusDidChange: NSNotification.Name

Posted when the status of the VPN connection changes.

### Handling errors

func fetchLastDisconnectError(completionHandler: ((any Error)?) -> Void)

Retrives the most recent error that caused the VPN to disconnect.

let NEVPNConnectionErrorDomain: String

The domain for errors resulting from VPN connection calls.

enum NEVPNConnectionError

Error codes specific to VPN connections.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NETunnelProviderSession

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### VPN control

class NETunnelProviderSession

An object to start and stop a tunnel connection and get its status.

