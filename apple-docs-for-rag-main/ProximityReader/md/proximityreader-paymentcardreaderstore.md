

- ProximityReader
-  PaymentCardReaderStore 

Structure

# PaymentCardReaderStore

A structure that manages the store that contains all the Store and Forward reads.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
struct PaymentCardReaderStore
```

## Topics

### Instance Methods

func fetchStoredPaymentCardReadResultBatch(size: Int) async throws -> StoreAndForwardBatch

Returns a batch of reads the framework previously stored, in chronological order, of the size you request.

func fetchStoredPaymentCardReadResultCount() async throws -> Int

Returns the number of reads the framework performed using a Store and Forward session.

func resetBatchState() async throws

Resets the current batch state in the store, allowing you to request a new batch.

func resolveBatch(batchDeletionToken: StoreAndForwardBatchDeletionToken) async throws -> Int

Deletes the current batch and all its Store and Forward payments, allowing you to request a new batch.

### Enumerations

enum StoreError

Values that describes errors related to the payments store.

## Relationships

### Conforms To

- Sendable

