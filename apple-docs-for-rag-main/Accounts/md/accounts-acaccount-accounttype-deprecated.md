

- Accounts
- ACAccount
-  accountType Deprecated

Instance Property

# accountType

The type of service account.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
var accountType: ACAccountType! { get set }
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Discussion

This property is required. You specify the account type using the init(accountType:) method. You can use the accounts(with:) method to retrieve all accounts of a particular type.

## See Also

### Accessing Properties

var accountDescription: String!

A human-readable description of the account.

Deprecated

var credential: ACAccountCredential!

The credential used to authenticate the user of this account.

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

