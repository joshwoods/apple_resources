

- Accounts
- ACAccount
-  credential Deprecated

Instance Property

# credential

The credential used to authenticate the user of this account.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
var credential: ACAccountCredential! { get set }
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Discussion

This property is required and must be set before the account is saved. For privacy reasons, this property is inaccessible after the account is saved.

## See Also

### Accessing Properties

var accountDescription: String!

A human-readable description of the account.

Deprecated

var accountType: ACAccountType!

The type of service account.

Deprecated

var identifier: NSString!

A unique identifier for this account.

Deprecated

var username: String!

The username for this account.

Deprecated

var userFullName: String!

The full name associated with the user account.

Deprecated

