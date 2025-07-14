

- Foundation
- URLProtectionSpace
-  serverTrust 

Instance Property

# serverTrust

A representation of the server’s SSL transaction state.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var serverTrust: SecTrust? { get }
```

## Mentioned in 

Performing manual server trust authentication

## Discussion

This value is `nil` if the authentication method of the protection space is not server trust.

## See Also

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

