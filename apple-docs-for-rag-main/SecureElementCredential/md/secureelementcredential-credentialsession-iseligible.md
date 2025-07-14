

- SecureElementCredential
- CredentialSession
-  isEligible 

Type Property

# isEligible

Clients should always check if this variable returns true to dynamically determine if the current device and user configuration can utilize this service before starting a session with this client

iOS 18.1+iPadOS 18.1+

``` source
static var isEligible: Bool { get async throws }
```

## Mentioned in 

Accessing and using secure element credentials

