

- Core Data
- NSPersistentHistoryTransaction
-  bundleID 

Instance Property

# bundleID

The originating bundle’s identifier.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var bundleID: String { get }
```

## Mentioned in 

Consuming relevant store changes

## See Also

### Inspecting Transaction Details

var author: String?

A granular description of the context that made the persistent history change, if available.

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

