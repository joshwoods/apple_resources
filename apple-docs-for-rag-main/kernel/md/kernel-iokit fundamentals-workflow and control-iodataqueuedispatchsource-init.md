

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODataQueueDispatchSource
-  init 

Instance Method

# init

Handles the basic initialization of the dispatch source.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
virtual bool init(void);
```

## Return Value

`true` if initialization was successful, or `false` if an error occurred.

## Discussion

Don't call this method directly. Call Create when you want to create a new data-queue dispatch source.

## See Also

### Configuring the Dispatch Source

+ Create

Creates a dispatch source that you use as a shared-memory data queue.

- free

Performs any final cleanup for the data-queue dispatch source.

