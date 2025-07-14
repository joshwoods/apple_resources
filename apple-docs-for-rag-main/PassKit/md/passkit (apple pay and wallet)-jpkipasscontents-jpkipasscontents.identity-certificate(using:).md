

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Identity
-  certificate(using:) 

Instance Method

# certificate(using:)

The certificate associated with the Identity.

iOS 18.0+iPadOS 18.0+

``` source
func certificate(using request: JPKIPassContents.AuthenticationRequest) async throws -> JPKIPassContents.Certificate
```

**Required**

## Parameters 

`request`  

The person’s authentication request used to perform the Identity certificate.

## See Also

### Data associated with the identity

associatedtype IdentityType : JPKIPassContents.Identity

The type associated with the protocol.

**Required**

