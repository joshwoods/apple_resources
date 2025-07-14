

- Video Subscriber Account
-  VSUserAccountManager 

Class

# VSUserAccountManager

The object that coordinates your app’s user account actions.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+

``` source
class VSUserAccountManager
```

## Overview

Don’t create `VSUserAccountManager` directly; use shared.

## Topics

### Getting the account manager

class var shared: VSUserAccountManager

A shared instance of the user account manager class.

### Getting user accounts

func userAccounts(options: VSUserAccountManager.QueryOptions) async throws -> [VSUserAccount]

Returns a list of registered user accounts for your app.

struct QueryOptions

Constants that represent options you use to fetch a list of user accounts.

### Updating a user account

func update(VSUserAccount) async throws

Registers a new user account.

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

### User account management

struct VSUserAccount

An object that represents a user’s account.

