

- FinanceKit
-  FinanceError 

Enumeration

# FinanceError

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum FinanceError
```

## Topics

### Operators

static func == (FinanceError, FinanceError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case dataRestricted(FinanceStore.DataType)

The data is in a restricted state.

case historyTokenInvalid

case unknown

An unknown error occurred.

### Instance Properties

var errorCode: Int

The error code within the given domain.

var errorDescription: String?

A localized message that describes what error occurred.

var errorUserInfo: [String : Any]

The user-info dictionary that contains additional information about the error.

var failureReason: String?

A localized message that describes the reason for the failure

### Type Properties

static var errorDomain: String

The domain of the error.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- LocalizedError
- Sendable

