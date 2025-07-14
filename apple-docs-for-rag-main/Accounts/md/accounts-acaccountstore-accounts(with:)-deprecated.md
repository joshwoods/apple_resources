

- Accounts
- ACAccountStore
-  accounts(with:) Deprecated

Instance Method

# accounts(with:)

Returns all accounts of the specified type.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
func accounts(with accountType: ACAccountType!) -> [Any]!
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Parameters 

`accountType`  

The type of an account.

## Return Value

All accounts that match `accountType`.

## See Also

### Getting Accounts

var accounts: NSArray!

The accounts managed by this account store.

Deprecated

func account(withIdentifier: String!) -> ACAccount!

Returns the account with the specified identifier.

Deprecated

