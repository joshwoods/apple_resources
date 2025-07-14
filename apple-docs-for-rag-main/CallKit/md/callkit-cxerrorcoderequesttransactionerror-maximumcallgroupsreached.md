

- CallKit
- CXErrorCodeRequestTransactionError
-  maximumCallGroupsReached 

Type Property

# maximumCallGroupsReached

Performing the requested transaction exceeds the maximum number of call groups for the provider.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
static var maximumCallGroupsReached: CXErrorCodeRequestTransactionError.Code { get }
```

## See Also

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

