

- AdAttributionKit
- AppImpression
-  init(compactJWS:) 

Initializer

# init(compactJWS:)

Creates a new app impression with the provided compact JSON Web Signature (JWS).

iOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
init(compactJWS: String) async throws
```

## Parameters 

`compactJWS`  

A string that represents a JWS.

## Discussion

Create a new `AppImpression` by providing a compact string representation of the JWS as the following example shows:

```
    do {
        let impression = try await AppImpression(compactJWS: compactJWS)
        print("Impression advertised item ID: \(impression.advertisedItemID)")
    }
    catch {
        print("Failed to decode impression: \(error)")
    }
```

