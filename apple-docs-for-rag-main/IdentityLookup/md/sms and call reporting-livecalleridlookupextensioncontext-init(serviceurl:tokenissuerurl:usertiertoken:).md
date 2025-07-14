

- SMS and Call Reporting
- LiveCallerIDLookupExtensionContext
-  init(serviceURL:tokenIssuerURL:userTierToken:) 

Initializer

# init(serviceURL:tokenIssuerURL:userTierToken:)

Creates the app extension context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    serviceURL: URL,
    tokenIssuerURL: URL,
    userTierToken: Data
)
```

## Parameters 

`serviceURL`  

The endpoint of the service that the system uses to fetch identity and blocking information.

`tokenIssuerURL`  

The URL of the Privacy Pass token issuer.

`userTierToken`  

The system sends this token to the Privacy Pass token issuer, which can verify whether it belongs to a valid user of the app. It then issues a Privacy Pass token.

