

- CallKit
- CXErrorCodeRequestTransactionError
-  CXErrorCodeRequestTransactionError.Code 

Enumeration

# CXErrorCodeRequestTransactionError.Code

Error codes for the CallKit error domain.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
enum Code
```

## Topics

### Constants

case unknown

An unknown error occurred.

case unentitled

The app isn’t entitled to perform the actions in the requested transaction.

case unknownCallProvider

The controller couldn’t find a call provider to perform the actions in the requested transaction.

case emptyTransaction

The requested transaction contains no actions.

case unknownCallUUID

The requested transaction contains call actions that reference an unknown UUID.

case callUUIDAlreadyExists

The requested transaction contains call actions that reference a UUID that already exists.

case invalidAction

The requested transaction contains an invalid action.

case maximumCallGroupsReached

The requested transaction contains actions that, if performed, would exceed the maximum number of call groups for the provider.

### Enumeration Cases

case callIsProtected

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct CXErrorCodeRequestTransactionError

let CXErrorDomainRequestTransaction: String

Domain for errors when requesting a transaction from a call controller.

