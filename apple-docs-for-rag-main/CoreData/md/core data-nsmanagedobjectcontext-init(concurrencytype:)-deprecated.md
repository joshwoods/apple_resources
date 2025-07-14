

- Core Data
- NSManagedObjectContext
-  init(concurrencyType:) Deprecated

Initializer

# init(concurrencyType:)

Creates a context that uses the specified concurrency type.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(concurrencyType ct: NSManagedObjectContextConcurrencyType)
```

Deprecated

Use init(_:) instead.

## Parameters 

`ct`  

The context’s concurrency type. For possible values, see NSManagedObjectContextConcurrencyType.

## Mentioned in 

Using Core Data in the background

## Discussion

For more information, see Concurrency.

## See Also

### Creating a context

convenience init(NSManagedObjectContext.ConcurrencyType)

Creates a context that uses the specified concurrency type.

struct ConcurrencyType

The concurrency types to use with a managed object context.

enum NSManagedObjectContextConcurrencyType

The concurrency types you can use with a managed object context.

