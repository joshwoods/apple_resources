

- Accounts
- ACAccount
-  accountDescription Deprecated

Instance Property

# accountDescription

A human-readable description of the account.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
var accountDescription: String! { get set }
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Discussion

This property is available if the user grants the application access to this account; otherwise it’s `nil`.

## See Also

### Accessing Properties

var accountType: ACAccountType!

The type of service account.

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

