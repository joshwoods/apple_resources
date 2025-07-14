

- Core Data
- NSPersistentHistoryTransaction
-  entityDescription 

Type Property

# entityDescription

The entity description of the persistent history transaction entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class var entityDescription: NSEntityDescription? { get }
```

## Discussion

The entity description of NSPersistentHistoryTransaction lists the properties of the persistent history change. This can be useful for filtering your request.

## See Also

### Customizing History Fetch Requests

class var fetchRequest: NSFetchRequest&lt;any NSFetchRequestResult>?

A fetch request that has the persistent history transaction as the entity.

class func entityDescription(with: NSManagedObjectContext) -> NSEntityDescription?

Requests an entity description using the provided context for the managed object type affected by the transaction.

