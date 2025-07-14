

- Accounts
- ACAccountCredential
-  init(oAuthToken:tokenSecret:) Deprecated

Initializer

# init(oAuthToken:tokenSecret:)

Initializes an account credential using OAuth.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
init!(
    oAuthToken token: String!,
    tokenSecret secret: String!
)
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Parameters 

`token`  

The client application’s token.

`secret`  

The client application’s secret token.

## Return Value

Newly initialized account credential.

## Discussion

Accounts can optionally use the OAuth open authentication standard to authenticate your client application. Instead of the user giving their username and password to log in, the server authenticates the user, and your client application receives a token that grants it access to specific resources for a defined duration. The authentication mechanism uses a key and secret scheme similar to the public and private keys used by `ssh`. A token is a unique, random string of letters and numbers that’s paired with a secret to protect the token from being abused. You initialize account credentials using this token and secret token.

To learn more about OAuth, go to OAuth.

## See Also

### Initializing Credentials

init!(oAuth2Token: String!, refreshToken: String!, expiryDate: Date!)

Initializes an account credential using OAuth 2.

Deprecated

