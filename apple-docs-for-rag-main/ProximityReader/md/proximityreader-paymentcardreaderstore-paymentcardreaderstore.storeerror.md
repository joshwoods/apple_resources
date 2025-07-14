

- ProximityReader
- PaymentCardReaderStore
-  PaymentCardReaderStore.StoreError 

Enumeration

# PaymentCardReaderStore.StoreError

Values that describes errors related to the payments store.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
enum StoreError
```

## Topics

### Enumeration Cases

case busy

The store is busy executing a previous request.

case networkError

The user needs to be online to fetch or resolve a batch.

case notAllowed

An error that indicates there’s an entitlement issue, an invalid application bundle, or a configuration issue.

case passcodeDisabled

To fetch a batch device’s passcode needs to be enabled.

case storeAndForwardBatchAlreadyExists

An error that indicates that a previous batch exists in the store and needs to be resolved or reset prior the current fetch batch request.

case storeAndForwardBatchNotFound

The store does not have a batch.

case storeAndForwardBatchSizeInvalid

The requested batch size is invalid.

case storeAndForwardDeletionTokenExpired

The token provided is expired, refresh it and try again.

case storeAndForwardDeletionTokenInvalid

The token provided is invalid, try again.

case storeAndForwardResultsNotFound

The Store and Forward store is empty.

case unknown(code: Int)

An unexpected error happened, try again.

### Default Implementations

Error Implementations

## Relationships

### Conforms To

- Error
- Sendable

