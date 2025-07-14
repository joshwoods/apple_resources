

- Foundation
- URLCredential
-  persistence 

Instance Property

# persistence

The credential’s persistence setting.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var persistence: URLCredential.Persistence { get }
```

## See Also

### Getting credential properties

var user: String?

The credential’s user name.

var certificates: [Any]

The intermediate certificates of the credential, if it is a client certificate credential.

var hasPassword: Bool

A Boolean value that indicates whether the credential has a password.

var password: String?

The credential’s password.

var identity: SecIdentity?

The identity of this credential if it is a client certificate credential.

enum Persistence

Constants that specify how long the credential will be kept.

