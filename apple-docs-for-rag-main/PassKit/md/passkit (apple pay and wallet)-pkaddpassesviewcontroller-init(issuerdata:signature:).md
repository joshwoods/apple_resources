

- PassKit (Apple Pay and Wallet)
- PKAddPassesViewController
-  init(issuerData:signature:) 

Initializer

# init(issuerData:signature:)

Initializes and returns a new add-passes view controller with the issuer data, and signature you provide.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+visionOS 1.0+

``` source
@MainActor
init(
    issuerData: Data,
    signature: Data
) throws
```

## Parameters 

`issuerData`  

The NSData object that represents the issuer data.

`signature`  

The NSData object that represents the issuer’s signature.

## See Also

### Creating an add-passes view controller

init?(pass: PKPass)

Initializes and returns a newly created add-passes view controller with a single pass.

init?(passes: [PKPass])

Initializes and returns a newly created add-passes view controller with an array of passes.

