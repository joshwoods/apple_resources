

- Accounts
-  ACAccountType Deprecated

Class

# ACAccountType

An object that encapsulates information about all accounts of a particular type.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
class ACAccountType
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Overview

You don’t create account type objects directly. To obtain an account type object, use the accountType(withAccountTypeIdentifier:) method or the accountType property of an account object. Use the accounts(with:) method to obtain all accounts of a particular type.

## Topics

### Accessing Properties

var accessGranted: Bool

A Boolean value indicating whether the user granted the application access to accounts of this type.

var accountTypeDescription: String!

A human-readable description of the account type.

var identifier: String!

The unique identifier for the account type.

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

