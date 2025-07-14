

- StoreKit
- External Purchase
-  Receiving and decoding external purchase tokens 

Article

# Receiving and decoding external purchase tokens

Receive tokens for external purchases that you use to report transactions to Apple.

## Overview

An *external purchase token* is a unique string that your app or website receives when your app’s customer chooses to view your external purchase offerings. You receive external purchase tokens in two ways: within your app, or appended to your website URL for link out, as follows:

- In your app, the API returns the token when your app calls presentNoticeSheet() and the response is ExternalPurchase.NoticeResult.continuedWithExternalPurchaseToken(token:).

- For link out, when your app calls open() or open(url:), the API appends the token to the current storefront’s destination URL that you configure in the SKExternalPurchaseLink or SKExternalPurchaseMultiLink property list keys, respectively.

- For custom link out, when your app configures the SKExternalPurchaseCustomLinkRegions property list key and calls the token(for:) function.

Decode the token to obtain its externalPurchaseId, which you use to report the tokens and associated transactions to Apple using the Send External Purchase Report endpoint of the External Purchase Server API.

### Decode external purchase tokens

The token your app or website’s server receives is a string that is Base64URL-encoded JSON. Decode the token using Base64URL decoding to read the JSON, which contains the following fields:

- The `appAppleId` and `bundleId`, which uniquely identify the app to which the token applies

- The `tokenCreationDate`, which is the UNIX time, in milliseconds, when the system created the token

- The `externalPurchaseId`, which is a unique value the system created to identify the token

For custom link out, the token is represented by ExternalPurchaseCustomLink.Token and has two additional fields:

- A `tokenType`, which has a value of `ACQUISITION` or `SERVICES`

- A `tokenExpirationDate`, which is the UNIX time, in milliseconds, when the token expires, after which you no longer associate the token with new transactions

The `externalPurchaseId` field is required by the Send External Purchase Report endpoint when you report tokens and transactions. To get the `externalPurchaseId`, follow these steps:

- Decode the token string using Base64URL decoding. For example, if the token string is:

`ewoJImFwcEFwcGxlSWQiOjEyMzQ1Njc4OTAsCgkiYnVuZGxlSWQiOiJjb20uZXhhbXBsZSIsCgkidG9rZW5DcmVhdGlvbkRhdGUiOjE3MDYxNjk2MDAwMDAsCgkiZXh0ZXJuYWxQdXJjaGFzZUlkIjoiMDAwMDAwMDAtMDAwMC0wMDAwLTAwMDAtMDAwMDAwMDAwMDAwIgp9`

Then, the token’s value after Base64URL decoding is the following JSON:

```
{  
  "appAppleId":1234567890,  
  "bundleId":"com.example",  
  "tokenCreationDate":1706169600000,
  "externalPurchaseId":"00000000-0000-0000-0000-000000000000"
}
```

- Use the value of the `externalPurchaseId` property to identify the token when you call the Send External Purchase Report endpoint.

### Recognize tokens from the testing environment

The External Purchase API returns external purchase tokens that are specific to the app’s environment: production or sandbox. You can recognize a token for the sandbox environment by its `externalPurchaseId` property, which always begins with “`SANDBOX`”.

The following example is an external purchase token that the system created in the sandbox environment. The sandbox token string is:

`ewoJImFwcEFwcGxlSWQiOjEyMzQ1Njc4OTAsCgkiYnVuZGxlSWQiOiJjb20uZXhhbXBsZSIsCgkidG9rZW5DcmVhdGlvbkRhdGUiOjE3MDYxNjk2MDAwMDAsCgkiZXh0ZXJuYWxQdXJjaGFzZUlkIjoiU0FOREJPWF8wMDAwMDAwMC0wMDAwLTAwMDAtMDAwMC0wMDAwMDAwMDAwMDAiCn0K`

The token’s JSON content after Base64URL decoding is:

```
{
    "appAppleId":1234567890,
    "bundleId":"com.example",
    "tokenCreationDate":1706169600000,
    "externalPurchaseId":"SANDBOX_00000000-0000-0000-0000-000000000000"
}
```

The `externalPurchaseId` includes the “`SANDBOX`” prefix in the testing environment.

