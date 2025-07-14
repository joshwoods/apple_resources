

- Core Data
- NSPersistentHistoryTransaction
-  fetchRequest 

Type Property

# fetchRequest

A fetch request that has the persistent history transaction as the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class var fetchRequest: NSFetchRequest? { get }
```

## See Also

### Customizing History Fetch Requests

class var entityDescription: NSEntityDescription?

The entity description of the persistent history transaction entity.

class func entityDescription(with: NSManagedObjectContext) -> NSEntityDescription?

Requests an entity description using the provided context for the managed object type affected by the transaction.

