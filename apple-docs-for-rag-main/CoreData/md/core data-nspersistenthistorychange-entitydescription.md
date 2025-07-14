

- Core Data
- NSPersistentHistoryChange
-  entityDescription 

Type Property

# entityDescription

The entity description of the persistent history change entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class var entityDescription: NSEntityDescription? { get }
```

## Discussion

The entity description of a NSPersistentHistoryChange, includes its properties, which can be useful for filtering your persistent history change request.

## See Also

### Inspecting Change Metadata

class var fetchRequest: NSFetchRequest&lt;any NSFetchRequestResult>?

A fetch request that has the persistent history change as the entity.

class func entityDescription(with: NSManagedObjectContext) -> NSEntityDescription?

Requests an entity description for the managed object type affected by the change using the provided context.

