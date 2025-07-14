

- StoreKit
- ExternalPurchaseCustomLink
-  token(for:) 

Type Method

# token(for:)

Requests an external purchase token of the specified type.

iOS 18.1+iPadOS 18.1+macOS 15.1+tvOS 18.1+visionOS 2.1+watchOS 11.1+

``` source
static func token(for tokenType: String) async throws -> ExternalPurchaseCustomLink.Token?
```

## Parameters 

`tokenType`  

A string that indicates the token type. Valid string values are: `ACQUISITION`, `SERVICES`

## Return Value

Returns an external purchase token of the type you specify, or returns `nil` if there isn’t an active token of the specified type. This method throws an error if your app isn’t eligible to use this API.

## Mentioned in 

Receiving and decoding external purchase tokens

## Discussion

Use this method if your app configures the SKExternalPurchaseCustomLinkRegions property list key.

Request both token types when your app launches and immediately associate the tokens with a customer account on your server. You can also call this method at any other time, such as before offering external purchases. The method returns the same token, of each type, until it expires.

Decode the token to read its contents, including the expiration date. For more information, see Receiving and decoding external purchase tokens. For a code example that shows requesting the tokens, see ExternalPurchaseCustomLink.

Report tokens and all transactions associated with the tokens from your server, using the External Purchase Server API.

## See Also

### Getting external purchase tokens

struct Token

An external purchase token for use with custom links.

