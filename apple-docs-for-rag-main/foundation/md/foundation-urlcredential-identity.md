

- Foundation
- URLCredential
-  identity 

Instance Property

# identity

The identity of this credential if it is a client certificate credential.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var identity: SecIdentity? { get }
```

## Discussion

This value is `nil` if the credential is not a client certificate credential.

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

var persistence: URLCredential.Persistence

The credential’s persistence setting.

enum Persistence

Constants that specify how long the credential will be kept.

