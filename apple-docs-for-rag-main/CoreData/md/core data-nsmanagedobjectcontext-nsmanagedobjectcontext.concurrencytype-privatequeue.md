

- Core Data
- NSManagedObjectContext
- NSManagedObjectContext.ConcurrencyType
-  privateQueue 

Type Property

# privateQueue

A concurrency type where the context performs its tasks on a private queue.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static let privateQueue: NSManagedObjectContext.ConcurrencyType
```

## See Also

### Concurrency Types

static let mainQueue: NSManagedObjectContext.ConcurrencyType

A concurrency type where the context performs its tasks on the main queue.

