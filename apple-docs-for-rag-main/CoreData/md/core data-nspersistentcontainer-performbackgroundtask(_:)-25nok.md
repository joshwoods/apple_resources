

- Core Data
- NSPersistentContainer
-  performBackgroundTask(\_:) 

Instance Method

# performBackgroundTask(\_:)

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func performBackgroundTask(_ block: @escaping (NSManagedObjectContext) throws -> T) async rethrows -> T
```

## See Also

### Performing Background Tasks

func performBackgroundTask((NSManagedObjectContext) -> Void)

Executes a closure on a private queue using an ephemeral managed object context.

