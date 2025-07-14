

- File Provider
- NSFileProviderManager
-  run(\_:) 

Instance Method

# run(\_:)

Asks the system to schedule and execute the specified operations.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
func run(_ operations: [any NSFileProviderTestingOperation]) throws -> [AnyHashable : any Error]
```

## Parameters 

`operations`  

An array of operations. Populate this array with one or more operations returned by the listAvailableTestingOperations() method.

## Discussion

Important

Before calling this method, you must set the domain’s testingModes property to include the interactive value.

The system waits until all of the specified operations complete and reports an error for any operations that fail.

## See Also

### Testing

func listAvailableTestingOperations() throws -> [any NSFileProviderTestingOperation]

Lists all the operations that are ready for scheduling.

