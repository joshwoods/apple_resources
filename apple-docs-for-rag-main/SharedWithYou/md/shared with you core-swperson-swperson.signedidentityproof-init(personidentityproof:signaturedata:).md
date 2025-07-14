

- Shared With You Core
- SWPerson
- SWPerson.SignedIdentityProof
-  init(personIdentityProof:signatureData:) 

Initializer

# init(personIdentityProof:signatureData:)

Creates and intializes a signed identity object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    personIdentityProof: SWPerson.IdentityProof,
    signatureData data: Data
)
```

## Parameters 

`personIdentityProof`  

The SWPerson.IdentityProof the system uses to create the signed identity.

`data`  

The data for the signature.

