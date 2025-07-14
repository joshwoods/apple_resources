

- Core Data
-  NSPersistentHistoryTransaction 

Class

# NSPersistentHistoryTransaction

A set of changes in the persistent history based on a context save or batch operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class NSPersistentHistoryTransaction
```

## Mentioned in 

Consuming relevant store changes

## Topics

### Requesting Notifications

func objectIDNotification() -> Notification

Obtains a notification for use in merging the transaction’s changes into a managed object context.

### Customizing History Fetch Requests

class var fetchRequest: NSFetchRequest&lt;any NSFetchRequestResult>?

A fetch request that has the persistent history transaction as the entity.

class var entityDescription: NSEntityDescription?

The entity description of the persistent history transaction entity.

class func entityDescription(with: NSManagedObjectContext) -> NSEntityDescription?

Requests an entity description using the provided context for the managed object type affected by the transaction.

### Inspecting Transaction Details

var author: String?

A granular description of the context that made the persistent history change, if available.

var bundleID: String

The originating bundle’s identifier.

var changes: [NSPersistentHistoryChange]?

The array of persistent history changes.

var contextName: String?

The originating context’s name.

var processID: String

The originating process’s identifier.

var storeID: String

The originating store’s identifier.

var timestamp: Date

The date of the persistent history change.

var token: NSPersistentHistoryToken

The token that represents this transaction in the persistent history.

var transactionNumber: Int64

The transaction’s numeric identifier.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Reading History

class NSPersistentHistoryChange

A change representing the insertion, update, or deletion of a managed object in the persistent store.

