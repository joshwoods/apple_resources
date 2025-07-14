

- CallKit
- CXErrorCodeRequestTransactionError
- CXErrorCodeRequestTransactionError.Code
-  CXErrorCodeRequestTransactionError.Code.emptyTransaction 

Case

# CXErrorCodeRequestTransactionError.Code.emptyTransaction

The requested transaction contains no actions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
case emptyTransaction
```

## See Also

### Constants

case unknown

An unknown error occurred.

case unentitled

The app isn’t entitled to perform the actions in the requested transaction.

case unknownCallProvider

The controller couldn’t find a call provider to perform the actions in the requested transaction.

case unknownCallUUID

The requested transaction contains call actions that reference an unknown UUID.

case callUUIDAlreadyExists

The requested transaction contains call actions that reference a UUID that already exists.

case invalidAction

The requested transaction contains an invalid action.

case maximumCallGroupsReached

The requested transaction contains actions that, if performed, would exceed the maximum number of call groups for the provider.

