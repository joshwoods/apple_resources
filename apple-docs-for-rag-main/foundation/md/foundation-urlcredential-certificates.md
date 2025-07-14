

- Foundation
- URLCredential
-  certificates 

Instance Property

# certificates

The intermediate certificates of the credential, if it is a client certificate credential.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var certificates: [Any] { get }
```

## Discussion

The certificates are SecCertificate objects representing the intermediate certificates of the credential. This value is `nil` if this is not a client certificate credential or if the credential was created with no intermediate certificates.

## See Also

### Getting credential properties

var user: String?

The credential’s user name.

var hasPassword: Bool

A Boolean value that indicates whether the credential has a password.

var password: String?

The credential’s password.

var identity: SecIdentity?

The identity of this credential if it is a client certificate credential.

var persistence: URLCredential.Persistence

The credential’s persistence setting.

enum Persistence

Constants that specify how long the credential will be kept.

