

- Accounts
- ACAccountCredential
-  init(oAuth2Token:refreshToken:expiryDate:) Deprecated

Initializer

# init(oAuth2Token:refreshToken:expiryDate:)

Initializes an account credential using OAuth 2.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
init!(
    oAuth2Token token: String!,
    refreshToken: String!,
    expiryDate: Date!
)
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Parameters 

`token`  

The client application’s token.

`refreshToken`  

The client application’s refresh token.

`expiryDate`  

The date the token expires.

## Discussion

Accounts can optionally use the OAuth open authentication standard to authenticate your client application. Instead of the user giving their username and password to log in, the server authenticates the user, and your client application receives a token that grants it access to specific resources for a defined duration. The authentication mechanism uses a key and secret scheme similar to the public and private keys used by `ssh`. A token is a unique, random string of letters and numbers that’s paired with a secret to protect the token from being abused. You initialize account credentials using this token and secret token.

To learn more about OAuth, go to OAuth.

## See Also

### Initializing Credentials

init!(oAuthToken: String!, tokenSecret: String!)

Initializes an account credential using OAuth.

Deprecated

