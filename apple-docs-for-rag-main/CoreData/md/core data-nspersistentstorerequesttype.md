

- Core Data
-  NSPersistentStoreRequestType 

Enumeration

# NSPersistentStoreRequestType

Constants that specify the types of fetch requests.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum NSPersistentStoreRequestType
```

## Overview

requestType uses these constants.

## Topics

### Constants

case fetchRequestType

Specifies that the request returns managed objects.

case saveRequestType

Specifies that the request saves managed objects.

case batchInsertRequestType

A request that inserts data into a persistent store using a batch of managed objects or dictionaries.

case batchUpdateRequestType

A request that updates data for multiple managed objects in a persistent store.

case batchDeleteRequestType

A request that deletes data for multiple managed objects from a persistent store.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring a Request

var affectedStores: [NSPersistentStore]?

The stores the request should be sent to.

var requestType: NSPersistentStoreRequestType

The type of the fetch request.

