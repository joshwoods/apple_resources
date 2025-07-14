

- Core Data
- NSManagedObjectContext
-  NSManagedObjectContext.ConcurrencyType 

Structure

# NSManagedObjectContext.ConcurrencyType

The concurrency types to use with a managed object context.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct ConcurrencyType
```

## Topics

### Concurrency Types

static let mainQueue: NSManagedObjectContext.ConcurrencyType

A concurrency type where the context performs its tasks on the main queue.

static let privateQueue: NSManagedObjectContext.ConcurrencyType

A concurrency type where the context performs its tasks on a private queue.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable

## See Also

### Creating a context

convenience init(NSManagedObjectContext.ConcurrencyType)

Creates a context that uses the specified concurrency type.

init(concurrencyType: NSManagedObjectContextConcurrencyType)

Creates a context that uses the specified concurrency type.

Deprecated

enum NSManagedObjectContextConcurrencyType

The concurrency types you can use with a managed object context.

