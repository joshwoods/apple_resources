

- Foundation
- URLProtectionSpace
-  authenticationMethod 

Instance Property

# authenticationMethod

The authentication method used by the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var authenticationMethod: String { get }
```

## Mentioned in 

Performing manual server trust authentication

## Discussion

The supported authentication methods are listed in NSURLProtectionSpace authentication method constants.

## See Also

### Getting protection space properties

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

