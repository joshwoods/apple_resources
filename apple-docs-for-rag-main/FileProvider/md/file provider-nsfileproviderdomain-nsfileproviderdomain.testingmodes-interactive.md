

- File Provider
- NSFileProviderDomain
- NSFileProviderDomain.TestingModes
-  interactive 

Type Property

# interactive

A testing mode where the extension can deterministically test asynchronous operations.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
static var interactive: NSFileProviderDomain.TestingModes { get }
```

## Discussion

Disable the system’s automatic scheduling and execution of operations. Instead, the File Provider extension can manually determine the order of execution.

This testing mode enables the following synchronous methods:

listAvailableTestingOperations()  
Lists all the operations that are ready for scheduling.

run(_:)  
Asks the system to schedule and execute the specified operations.

The interactive testing mode expects the File Provider extension to repeat the following steps while running tests:

1.  Call listAvailableTestingOperations()to get the list of outstanding operations.

2.  Select the next set of operations required by your test.

3.  Call run(_:)to execute those operations.

The `interactive` testing mode also disables some of the File Provider extension’s crash guarantees. For example, the system may lose any event that it hasn’t yet ingested.

## See Also

### Accessing Modes

static var alwaysEnabled: NSFileProviderDomain.TestingModes

A testing mode that automatically enables the domain.

