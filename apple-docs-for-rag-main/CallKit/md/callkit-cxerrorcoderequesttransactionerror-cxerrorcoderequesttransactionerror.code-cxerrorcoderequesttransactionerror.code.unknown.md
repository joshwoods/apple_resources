

- CallKit
- CXErrorCodeRequestTransactionError
- CXErrorCodeRequestTransactionError.Code
-  CXErrorCodeRequestTransactionError.Code.unknown 

Case

# CXErrorCodeRequestTransactionError.Code.unknown

An unknown error occurred.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
case unknown
```

## See Also

### Constants

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

