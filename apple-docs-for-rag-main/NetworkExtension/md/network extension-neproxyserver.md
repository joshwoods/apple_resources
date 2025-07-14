

- Network Extension
-  NEProxyServer 

Class

# NEProxyServer

`NEProxyServer` contains settings for a proxy server.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEProxyServer
```

## Overview

`NEProxyServer` instances are used inside of NEProxySettings instances to configure proxy settings for VPN connections.

## Topics

### Initializing a Proxy Server

init(address: String, port: Int)

Initialize a newly-allocated `NEProxyServer` object

### Accessing Proxy Server Properties

var address: String

The address of the proxy server.

var port: Int

The TCP port on which the proxy server is listening for connections.

var authenticationRequired: Bool

A Boolean indicating if the server requires authentication credentials.

var username: String?

The username portion of the authentication credential to be used to authenticate with the proxy server.

var password: String?

The password portion of the authentication credential to be used to authenticate with the proxy server.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Accessing Manual Proxy Properties

var httpEnabled: Bool

A Boolean indicating if a static HTTP proxy will be used.

var httpServer: NEProxyServer?

An NEProxyServer object containing the static HTTP proxy server settings.

var httpsEnabled: Bool

A Boolean indicating if a static HTTPS proxy will be used.

var httpsServer: NEProxyServer?

An NEProxyServer object containing the static HTTPS proxy server settings.

