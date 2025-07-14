

- SecureElementCredential
- CredentialSession
- CredentialSession.State
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two values are equal.

iOS 18.1+iPadOS 18.1+

``` source
static func == (left: CredentialSession.State, right: CredentialSession.State) -> Bool
```

## Discussion

Two credential states are equal if they are the same enumeration case and, for wired and card emulation states, their associated CredentialSession.Credential values are equal.

