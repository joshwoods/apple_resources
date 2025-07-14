

- Accounts
-  ACAccountCredential Deprecated

Class

# ACAccountCredential

A credential object that encapsulates the information needed to authenticate a user.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
class ACAccountCredential
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Overview

To create an account credential that uses the OAuth open authentication standard, use the init(oAuthToken:tokenSecret:) method.

## Topics

### Initializing Credentials

init!(oAuthToken: String!, tokenSecret: String!)

Initializes an account credential using OAuth.

init!(oAuth2Token: String!, refreshToken: String!, expiryDate: Date!)

Initializes an account credential using OAuth 2.

### Accessing Credential Properties

var oauthToken: String!

The token used for the credential.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Account Management

class ACAccountStore

The object you use to request, manage, and store the user’s account information.

Deprecated

class ACAccount

The information associated with one of the user’s accounts.

Deprecated

