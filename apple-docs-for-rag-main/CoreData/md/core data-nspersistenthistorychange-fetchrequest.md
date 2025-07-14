

- Core Data
- NSPersistentHistoryChange
-  fetchRequest 

Type Property

# fetchRequest

A fetch request that has the persistent history change as the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class var fetchRequest: NSFetchRequest? { get }
```

## See Also

### Inspecting Change Metadata

class var entityDescription: NSEntityDescription?

The entity description of the persistent history change entity.

class func entityDescription(with: NSManagedObjectContext) -> NSEntityDescription?

Requests an entity description for the managed object type affected by the change using the provided context.

