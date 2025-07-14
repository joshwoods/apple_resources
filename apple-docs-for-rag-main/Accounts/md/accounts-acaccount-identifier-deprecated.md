

- Accounts
- ACAccount
-  identifier Deprecated

Instance Property

# identifier

A unique identifier for this account.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
weak var identifier: NSString! { get }
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Discussion

Use the account(withIdentifier:) method to get an account with the specified identifier.

## See Also

### Accessing Properties

var accountDescription: String!

A human-readable description of the account.

Deprecated

var accountType: ACAccountType!

The type of service account.

Deprecated

var credential: ACAccountCredential!

The credential used to authenticate the user of this account.

Deprecated

var username: String!

The username for this account.

Deprecated

var userFullName: String!

The full name associated with the user account.

Deprecated

