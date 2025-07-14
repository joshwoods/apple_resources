

- Core Data
- NSPersistentContainer
-  performBackgroundTask(\_:) 

Instance Method

# performBackgroundTask(\_:)

Executes a closure on a private queue using an ephemeral managed object context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func performBackgroundTask(_ block: @escaping (NSManagedObjectContext) -> Void)
```

## Parameters 

`block`  

A closure that is executed by the persistent container against a newly created private context. The private context is passed into the block as part of the execution of the block.

## Mentioned in 

Using Core Data in the background

## Discussion

Each time this method is invoked, the persistent container creates a new NSManagedObjectContext with the concurrencyType set to NSManagedObjectContextConcurrencyType.privateQueueConcurrencyType. The persistent container then executes the passed in block against that newly created context on the context’s private queue.

## See Also

### Performing Background Tasks

func performBackgroundTask&lt;T>((NSManagedObjectContext) throws -> T) async rethrows -> T

