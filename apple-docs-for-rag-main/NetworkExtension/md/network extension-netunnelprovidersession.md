

- Network Extension
-  NETunnelProviderSession 

Class

# NETunnelProviderSession

An object to start and stop a tunnel connection and get its status.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NETunnelProviderSession
```

## Overview

`NETunnelProviderSession` objects control network tunnel connections provided by Tunnel Provider extensions.

`NETunnelProviderSession` objects are not instantiated directly. Instead, each NETunnelProviderManager object has an associated `NETunnelProviderSession` as a read-only property.

## Topics

### Controlling the tunnel connection

func startTunnel(options: [String : Any]?) throws

Start the process of connecting the tunnel.

func stopTunnel()

Start the process of disconnecting the tunnel.

### Communicating with the tunnel provider

func sendProviderMessage(Data, responseHandler: ((Data?) -> Void)?) throws

Send a message to the Tunnel Provider extension. If the extension is not running, it should be launched to handle the message. If this method can’t start sending the message it reports an error in the `returnError` parameter. If an error occurs while sending the message or returning the result, `nil` should be sent to the response handler as notification.

## Relationships

### Inherits From

- NEVPNConnection

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### VPN control

class NEVPNConnection

An object to start and stop a Personal VPN connection and get its status.

