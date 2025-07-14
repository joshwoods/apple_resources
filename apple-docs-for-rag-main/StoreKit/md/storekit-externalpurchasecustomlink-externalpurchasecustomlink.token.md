

- StoreKit
- ExternalPurchaseCustomLink
-  ExternalPurchaseCustomLink.Token 

Structure

# ExternalPurchaseCustomLink.Token

An external purchase token for use with custom links.

iOS 18.1+iPadOS 18.1+macOS 15.1+tvOS 18.1+visionOS 2.1+watchOS 11.1+

``` source
struct Token
```

## Mentioned in 

Receiving and decoding external purchase tokens

## Overview

StoreKit returns an external purchase token of this type when you call the token(for:) function. Your app gets these tokens if it configures the SKExternalPurchaseCustomLinkRegions property list key and uses the ExternalPurchaseCustomLink API.

For more information about tokens, see Receiving and decoding external purchase tokens.

## Topics

### Getting the token value

let value: String

A Base64URL-encoded JSON string that represents the external purchase token.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Offering external purchases with custom links

enum ExternalPurchaseCustomLink

Enables qualifying apps to offer custom links for external purchases.

com.apple.developer.storekit.external-purchase-link

A Boolean value that indicates whether your app can include a link that directs people to a website to make an external purchase.

SKExternalPurchaseCustomLinkRegions

An array of country code strings that indicate the regions where your app supports custom links for external purchases.

