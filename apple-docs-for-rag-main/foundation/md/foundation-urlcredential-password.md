

- Foundation
- URLCredential
-  password 

Instance Property

# password

The credential’s password.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var password: String? { get }
```

## Discussion

You should only access this property if you need the actual password value. If you only need to know if there is a password, use hasPassword. Accessing this property may result in prompting the user for access—for example, if the password is stored in the user’s keychain.

## See Also

### Getting credential properties

var user: String?

The credential’s user name.

var certificates: [Any]

The intermediate certificates of the credential, if it is a client certificate credential.

var hasPassword: Bool

A Boolean value that indicates whether the credential has a password.

var identity: SecIdentity?

The identity of this credential if it is a client certificate credential.

var persistence: URLCredential.Persistence

The credential’s persistence setting.

enum Persistence

Constants that specify how long the credential will be kept.

