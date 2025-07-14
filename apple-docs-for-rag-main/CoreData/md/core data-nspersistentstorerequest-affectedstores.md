

- Core Data
- NSPersistentStoreRequest
-  affectedStores 

Instance Property

# affectedStores

The stores the request should be sent to.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var affectedStores: [NSPersistentStore]? { get set }
```

## Discussion

The array contains instances of NSPersistentStore.

## See Also

### Related Documentation

Core Data Programming Guide

### Configuring a Request

var requestType: NSPersistentStoreRequestType

The type of the fetch request.

enum NSPersistentStoreRequestType

Constants that specify the types of fetch requests.

