

- DriverKit
- IODataQueueDispatchSource
-  init 

Instance Method

# init

Handles the basic initialization of the dispatch source.

DriverKitiOSiPadOSmacOS

``` source
bool init();
```

## Return Value

`true` if initialization was successful, or `false` if an error occurred.

## Discussion

Don’t call this method directly. Call Create when you want to create a new data-queue dispatch source.

## See Also

### Configuring the Dispatch Source

Create

Creates a dispatch source that you use as a shared-memory data queue.

free

Performs any final cleanup for the data-queue dispatch source.

