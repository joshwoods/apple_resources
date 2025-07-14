

- CallKit
-  CXErrorCodeRequestTransactionError 

Structure

# CXErrorCodeRequestTransactionError

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
struct CXErrorCodeRequestTransactionError
```

## Topics

### Constants

static var unknown: CXErrorCodeRequestTransactionError.Code

An unknown error occurred.

static var unentitled: CXErrorCodeRequestTransactionError.Code

The app doesn’t have the entitlement to perform the actions in the requested transaction.

static var unknownCallProvider: CXErrorCodeRequestTransactionError.Code

The controller can’t find a call provider to perform the actions in the requested transaction.

static var emptyTransaction: CXErrorCodeRequestTransactionError.Code

The requested transaction doesn’t contain any actions.

static var unknownCallUUID: CXErrorCodeRequestTransactionError.Code

The requested transaction contains call actions that reference an unknown UUID.

static var callUUIDAlreadyExists: CXErrorCodeRequestTransactionError.Code

The requested transaction contains call actions that reference a UUID that already exists.

static var invalidAction: CXErrorCodeRequestTransactionError.Code

The requested transaction contains an invalid action.

static var maximumCallGroupsReached: CXErrorCodeRequestTransactionError.Code

Performing the requested transaction exceeds the maximum number of call groups for the provider.

### Enumerations

enum Code

Error codes for the CallKit error domain.

### Type Properties

static var callIsProtected: CXErrorCodeRequestTransactionError.Code

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Error codes for the CallKit error domain.

let CXErrorDomainRequestTransaction: String

Domain for errors when requesting a transaction from a call controller.

