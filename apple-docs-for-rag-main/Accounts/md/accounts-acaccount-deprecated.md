

- Accounts
-  ACAccount Deprecated

Class

# ACAccount

The information associated with one of the user’s accounts.

iOS 6.0–15.0DeprecatediPadOS 6.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.8–12.0Deprecated

``` source
class ACAccount
```

Deprecated

Use appropriate non-Apple SDK corresponding to the type of account you want to reference instead

## Overview

An ACAccount object encapsulates information about a user account stored in the Accounts database. You can create and retrieve accounts using an ACAccountStore object. The ACAccountStore object provides an interface to the persistent Accounts database. For each user, all account objects belong to a single ACAccountStore object.

## Topics

### Creating an Account Object

init!(accountType: ACAccountType!)

Initializes a new account of the specified type.

### Accessing Properties

var accountDescription: String!

A human-readable description of the account.

var accountType: ACAccountType!

The type of service account.

var credential: ACAccountCredential!

The credential used to authenticate the user of this account.

var identifier: NSString!

A unique identifier for this account.

var username: String!

The username for this account.

var userFullName: String!

The full name associated with the user account.

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

class ACAccountCredential

A credential object that encapsulates the information needed to authenticate a user.

Deprecated

