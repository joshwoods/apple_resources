

- Foundation
- Process
-  terminationHandler 

Instance Property

# terminationHandler

A completion block the system invokes when the task completes.

macOS 10.7+

``` source
var terminationHandler: ((Process) -> Void)? { get set }
```

## Discussion

The system passes the task object to the block to allow access to the task parameters, for example to determine if the task completed successfully.

This block isn’t guaranteed to be fully executed prior to waitUntilExit() returning.

