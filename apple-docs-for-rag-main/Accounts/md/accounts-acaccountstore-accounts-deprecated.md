

- Accounts
- ACAccountStore
-  accounts Deprecated

Instance Property

# accounts

The accounts managed by this account store.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
weak var accounts: NSArray! { get }
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## See Also

### Getting Accounts

func account(withIdentifier: String!) -> ACAccount!

Returns the account with the specified identifier.

Deprecated

func accounts(with: ACAccountType!) -> [Any]!

Returns all accounts of the specified type.

Deprecated

