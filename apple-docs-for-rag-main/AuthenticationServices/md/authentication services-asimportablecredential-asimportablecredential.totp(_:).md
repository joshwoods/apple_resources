

- Authentication Services
- ASImportableCredential
-  ASImportableCredential.totp(\_:) 

Case

# ASImportableCredential.totp(\_:)

A time-based one-time password (TOTP) credential.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
case totp(ASImportableCredential.TOTP)
```

## See Also

### Login credential types

case basicAuthentication(ASImportableCredential.BasicAuthentication)

A password credential.

struct BasicAuthentication

A type to represent a basic authentication password.

case passkey(ASImportableCredential.Passkey)

A passkey credential.

struct Passkey

A type to represent a passkey credential.

struct TOTP

A type to represent a time-based one-time password generator (TOTP).

