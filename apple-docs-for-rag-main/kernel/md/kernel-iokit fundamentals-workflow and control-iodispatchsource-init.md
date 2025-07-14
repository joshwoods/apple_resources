

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchSource
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

## See Also

### Configuring the Dispatch Source

- Cancel

Cancel all callbacks from the dispatch source.

- free

Performs any final cleanup for the dispatch source.

