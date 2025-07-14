

- Foundation
- URLCredential
-  hasPassword 

Instance Property

# hasPassword

A Boolean value that indicates whether the credential has a password.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hasPassword: Bool { get }
```

## Discussion

This value is true if the receiver has a password, false otherwise.

This method does not attempt to retrieve the password.

If this credential’s password is stored in the user’s keychain, password may return `nil` even if this method returns true—getting the password may fail, or the user may refuse access.

## See Also

### Getting credential properties

var user: String?

The credential’s user name.

var certificates: [Any]

The intermediate certificates of the credential, if it is a client certificate credential.

var password: String?

The credential’s password.

var identity: SecIdentity?

The identity of this credential if it is a client certificate credential.

var persistence: URLCredential.Persistence

The credential’s persistence setting.

enum Persistence

Constants that specify how long the credential will be kept.

