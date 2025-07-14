

- Open Directory
-  kODAuthenticationTypeSetCertificateHashAsCurrent 

Global Variable

# kODAuthenticationTypeSetCertificateHashAsCurrent

An authentication type to set the certificate using the authenticated user’s credentials.

Mac CatalystmacOS 10.7+

``` source
let kODAuthenticationTypeSetCertificateHashAsCurrent: String
```

## Discussion

The authentication array contains the following items (in order):

- The username in UTF-8 format

- Hashed certificate data (40 hex digits)

## See Also

### Constants

let kODAuthenticationType2WayRandom: String

The authentication type used to specify two way random authentication.

let kODAuthenticationType2WayRandomChangePasswd: String

The authentication type used to change a user’s password using two way random authentication.

let kODAuthenticationTypeAPOP: String

The authentication type used to specify APOP authentication.

let kODAuthenticationTypeCRAM_MD5: String

The authentication type used to specify CRAM MD5 authentication.

let kODAuthenticationTypeChangePasswd: String

The authentication type used to change a user’s password using CRAM MD5 authentication.

let kODAuthenticationTypeClearText: String

The authentication type used to specify cleartext authentication.

let kODAuthenticationTypeCrypt: String

The authentication type used to specify crypt authentication, which uses a crypt password stored in a user’s record if available.

let kODAuthenticationTypeDIGEST_MD5: String

The authentication type used to specify digest MD5 authentication.

let kODAuthenticationTypeDeleteUser: String

The authentication type used to specify that a user on an Apple password server be deleted.

let kODAuthenticationTypeGetEffectivePolicy: String

The authentication type used to access the policies applied to a user.

let kODAuthenticationTypeGetGlobalPolicy: String

The authentication type used to access the global authentication policy.

let kODAuthenticationTypeGetKerberosPrincipal: String

The authentication type used to access the name of the Kerberos principal.

let kODAuthenticationTypeGetPolicy: String

The authentication type used to specify that the plug-in should determine the authentication method to use.

let kODAuthenticationTypeGetUserData: String

The authentication type used to access user data on an Apple password server.

let kODAuthenticationTypeGetUserName: String

The authentication type used to access a username on an Apple password server.

