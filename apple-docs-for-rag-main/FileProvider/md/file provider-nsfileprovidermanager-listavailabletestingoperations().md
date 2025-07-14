

- File Provider
- NSFileProviderManager
-  listAvailableTestingOperations() 

Instance Method

# listAvailableTestingOperations()

Lists all the operations that are ready for scheduling.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
func listAvailableTestingOperations() throws -> [any NSFileProviderTestingOperation]
```

## Discussion

Important

Before calling this method, you must set the domain’s testingModes property to include the interactive value.

The system waits for all the pending disk and working set updates before returning the list of available operations. The operations that it returns may become invalid if the system receives new events, or when you schedule and execute operations using the run(_:) method.

## See Also

### Testing

func run([any NSFileProviderTestingOperation]) throws -> [AnyHashable : any Error]

Asks the system to schedule and execute the specified operations.

