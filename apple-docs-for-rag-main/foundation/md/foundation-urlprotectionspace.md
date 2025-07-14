

- Foundation
-  URLProtectionSpace 

Class

# URLProtectionSpace

A server or an area on a server, commonly referred to as a realm, that requires authentication.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLProtectionSpace
```

## Overview

A protection space defines a series of matching constraints that determine which credential should be provided. For example, if a request provides your delegate with a URLAuthenticationChallenge object that requests a client username and password, your app should provide the correct username and password for the particular host, port, protocol, and realm, as specified in the challenge’s protection space.

Note

This class has no designated initializer; its `init` method always returns `nil`. You must initialize this class by calling one of the initialization methods described in Creating a protection space.

## Topics

### Creating a protection space

init(host: String, port: Int, protocol: String?, realm: String?, authenticationMethod: String?)

Creates a protection space object from the given host, port, protocol, realm, and authentication method.

init(proxyHost: String, port: Int, type: String?, realm: String?, authenticationMethod: String?)

Creates a protection space object representing a proxy server.

### Getting protection space properties

var authenticationMethod: String

The authentication method used by the receiver.

var distinguishedNames: [Data]?

The acceptable certificate-issuing authorities for client certificate authentication.

var host: String

The receiver’s host.

var port: Int

The receiver’s port.

var `protocol`: String?

The receiver’s protocol.

var proxyType: String?

The receiver’s proxy type.

var realm: String?

The receiver’s authentication realm

var receivesCredentialSecurely: Bool

A Boolean value that indicates whether the credentials for the protection space can be sent securely.

var serverTrust: SecTrust?

A representation of the server’s SSL transaction state.

### Identifying protection space properties

NSURLProtectionSpace protocol types

These constants describe the supported protocols for a protection space, as returned by protocol.

NSURLProtectionSpace proxy types

These constants describe the supported proxy types used in init(proxyHost:port:type:realm:authenticationMethod:) and returned by proxyType.

NSURLProtectionSpace authentication method constants

Constants describing known values of the authenticationMethod property of a URLProtectionSpace.

### Instance Methods

func isProxy() -> Bool

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
- Sendable

## See Also

### Authentication and credentials

Handling an authentication challenge

Respond appropriately when a server demands authentication for a URL request.

class URLAuthenticationChallenge

A challenge from a server requiring authentication from the client.

class URLCredential

`A`n authentication credential consisting of information specific to the type of credential and the type of persistent storage to use, if any.

class URLCredentialStorage

The manager of a shared credentials cache.

