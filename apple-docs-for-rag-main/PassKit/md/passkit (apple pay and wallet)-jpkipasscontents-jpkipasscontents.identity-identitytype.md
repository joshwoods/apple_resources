

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Identity
-  IdentityType 

Associated Type

# IdentityType

The type associated with the protocol.

iOS 18.0+iPadOS 18.0+

``` source
associatedtype IdentityType : JPKIPassContents.Identity
```

**Required**

## See Also

### Data associated with the identity

func certificate(using: JPKIPassContents.AuthenticationRequest&lt;Self.IdentityType>) async throws -> JPKIPassContents.Certificate&lt;Self.IdentityType>

The certificate associated with the Identity.

**Required**

