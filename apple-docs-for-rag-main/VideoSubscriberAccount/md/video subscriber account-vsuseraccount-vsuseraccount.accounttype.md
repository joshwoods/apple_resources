

- Video Subscriber Account
- VSUserAccount
-  VSUserAccount.AccountType 

Enumeration

# VSUserAccount.AccountType

Constants that represent whether a user has access to paid content.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS

``` source
enum AccountType
```

## Overview

The default is VSUserAccount.AccountType.free.

## Topics

### Account types

case free

A constant that indicates a user has access to free content.

case paid

A constant that indicate a user has access to paid content.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating user accounts

init(accountType: VSUserAccount.AccountType, updateURL: URL?)

Creates a user account object with a URL for account update requests.

