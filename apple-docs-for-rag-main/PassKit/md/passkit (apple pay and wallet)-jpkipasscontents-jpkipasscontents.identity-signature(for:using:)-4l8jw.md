

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.Identity
-  signature(for:using:) 

Instance Method

# signature(for:using:)

Signs the supplied data with the identity’s private key

iOS 18.0+iPadOS 18.0+

``` source
func signature(
    for data: Data,
    using request: JPKIPassContents.AuthenticationRequest
) async throws -> JPKIPassContents.Signature
```

**Required**

## Discussion

- Properties:

  - data: Data to be signed with the specified identity

  - authentication: User authentication request to perform identity signature with

Throws

See Error type defined below

