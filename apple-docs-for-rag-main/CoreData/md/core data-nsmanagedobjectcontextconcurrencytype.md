

- Core Data
-  NSManagedObjectContextConcurrencyType 

Enumeration

# NSManagedObjectContextConcurrencyType

The concurrency types you can use with a managed object context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum NSManagedObjectContextConcurrencyType
```

## Topics

### Concurrency Types

case privateQueueConcurrencyType

Specifies that the context will be associated with a private dispatch queue.

case mainQueueConcurrencyType

Specifies that the context will be associated with the main queue.

case confinementConcurrencyType

Specifies that the context will use the thread confinement pattern.

Deprecated

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

### Creating a context

convenience init(NSManagedObjectContext.ConcurrencyType)

Creates a context that uses the specified concurrency type.

struct ConcurrencyType

The concurrency types to use with a managed object context.

init(concurrencyType: NSManagedObjectContextConcurrencyType)

Creates a context that uses the specified concurrency type.

Deprecated

