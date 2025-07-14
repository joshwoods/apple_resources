

- Accounts
-  ACAccountStore Deprecated

Class

# ACAccountStore

The object you use to request, manage, and store the user’s account information.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
class ACAccountStore
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Overview

The ACAccountStore class provides an interface for accessing, managing, and storing accounts. To create and retrieve accounts from the Accounts database, you must create an ACAccountStore object. Each ACAccount object belongs to a single account store object.

## Topics

### Requesting Access

func requestAccessToAccounts(with: ACAccountType!, options: [AnyHashable : Any]!, completion: ACAccountStoreRequestAccessCompletionHandler!)

Obtains permission to access protected user properties.

typealias ACAccountStoreRequestAccessCompletionHandler

Specifies a handler to call when access is granted or denied.

### Getting Accounts

var accounts: NSArray!

The accounts managed by this account store.

func account(withIdentifier: String!) -> ACAccount!

Returns the account with the specified identifier.

func accounts(with: ACAccountType!) -> [Any]!

Returns all accounts of the specified type.

### Getting Account Types

func accountType(withAccountTypeIdentifier: String!) -> ACAccountType!

Returns an account type that matches the specified identifier.

### Saving Accounts

func saveAccount(ACAccount!, withCompletionHandler: ACAccountStoreSaveCompletionHandler!)

Saves an account to the Accounts database.

typealias ACAccountStoreSaveCompletionHandler

Specifies a handler to call when an Accounts database operation is complete.

### Renewing Account Credentials

func renewCredentials(for: ACAccount!, completion: ACAccountStoreCredentialRenewalHandler!)

Renews account credentials when the credentials are no longer valid.

typealias ACAccountStoreCredentialRenewalHandler

Specifies a handler to call when credentials are renewed.

enum ACAccountCredentialRenewResult

Status codes of credential renewal requests.

### Removing Accounts

func removeAccount(ACAccount!, withCompletionHandler: ACAccountStoreRemoveCompletionHandler!)

Removes an account from the account store.

typealias ACAccountStoreRemoveCompletionHandler

Specifies a handler to call when an account is removed from the store.

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

class ACAccount

The information associated with one of the user’s accounts.

Deprecated

class ACAccountCredential

A credential object that encapsulates the information needed to authenticate a user.

Deprecated

