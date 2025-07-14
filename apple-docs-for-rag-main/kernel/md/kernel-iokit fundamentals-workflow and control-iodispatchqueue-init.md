

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchQueue
-  init 

Instance Method

# init

Initializes the dispatch queue object.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
virtual bool init(void);
```

## Return Value

`true` if initialization was successful, or `false` if it was unsuccessful.

## Discussion

Do not call this method directly. Call Create when you want to create a new dispatch queue.

## See Also

### Creating a Dispatch Queue

+ Create

Creates a new dispatch queue object.

- free

Performs any final cleanup for the dispatch queue object.

