

- SMS and Call Reporting
- LiveCallerIDLookupExtensionContext
-  userTierToken 

Instance Property

# userTierToken

An HTTP bearer token that authenticates the person using your app.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
let userTierToken: Data
```

## Mentioned in 

Getting up-to-date calling and blocking information for your app

## Discussion

The system sends this token to the Privacy Pass token issuer, which can verify whether it belongs to a valid user of your app. It then issues a Privacy Pass token.

## See Also

### Configuring the system

let serviceURL: URL

The endpoint of the service to fetch identity and blocking information.

let tokenIssuerURL: URL

The URL of the Privacy Pass token issuer.

