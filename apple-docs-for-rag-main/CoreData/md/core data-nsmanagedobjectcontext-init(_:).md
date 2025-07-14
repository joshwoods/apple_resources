

- Core Data
- NSManagedObjectContext
-  init(\_:) 

Initializer

# init(\_:)

Creates a context that uses the specified concurrency type.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
convenience init(_ type: NSManagedObjectContext.ConcurrencyType)
```

## Parameters 

`type`  

The context’s concurrency type. For possible values, see NSManagedObjectContext.ConcurrencyType.

## Discussion

For more information, see Concurrency.

## See Also

### Creating a context

struct ConcurrencyType

The concurrency types to use with a managed object context.

init(concurrencyType: NSManagedObjectContextConcurrencyType)

Creates a context that uses the specified concurrency type.

Deprecated

enum NSManagedObjectContextConcurrencyType

The concurrency types you can use with a managed object context.

