

- Foundation
- URLProtectionSpace
-  distinguishedNames 

Instance Property

# distinguishedNames

The acceptable certificate-issuing authorities for client certificate authentication.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var distinguishedNames: [Data]? { get }
```

## Discussion

This value is `nil` if the authentication method of the protection space is not client certificate. The returned issuing authorities are encoded with Distinguished Encoding Rules (DER).

## See Also

### Getting protection space properties

var authenticationMethod: String

The authentication method used by the receiver.

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

