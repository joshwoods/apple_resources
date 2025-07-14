

- Accounts
- ACAccountStore
-  account(withIdentifier:) Deprecated

Instance Method

# account(withIdentifier:)

Returns the account with the specified identifier.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
func account(withIdentifier identifier: String!) -> ACAccount!
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Parameters 

`identifier`  

A unique identifier for an account.

## Return Value

The account that matches the value specified in `identifier`.

## See Also

### Getting Accounts

var accounts: NSArray!

The accounts managed by this account store.

Deprecated

func accounts(with: ACAccountType!) -> [Any]!

Returns all accounts of the specified type.

Deprecated

