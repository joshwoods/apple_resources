

- Core Data
- NSFetchRequest
-  execute() 

Instance Method

# execute()

Executes the fetch request against the managed object context that is associated with the current queue.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func execute() throws -> [ResultType]
```

## Discussion

Calling `execute` on an NSFetchRequest will cause the NSFetchRequest to run against the managed object context (NSManagedObjectContext) that is associated with the queue on which the `execute` is called.

