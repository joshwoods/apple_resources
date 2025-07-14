

- Core Data
- NSPersistentHistoryTransaction
-  entityDescription(with:) 

Type Method

# entityDescription(with:)

Requests an entity description using the provided context for the managed object type affected by the transaction.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func entityDescription(with context: NSManagedObjectContext) -> NSEntityDescription?
```

## Parameters 

`context`  

The managed object context for this request.

## Return Value

The entity description (NSEntityDescription) of the persistent history transaction entity.

## See Also

### Customizing History Fetch Requests

class var fetchRequest: NSFetchRequest&lt;any NSFetchRequestResult>?

A fetch request that has the persistent history transaction as the entity.

class var entityDescription: NSEntityDescription?

The entity description of the persistent history transaction entity.

