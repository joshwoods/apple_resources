

- Kernel
- IOKit Fundamentals
- Data Types
- OSAction
-  free 

Instance Method

# free

Performs any final cleanup for the action object.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
virtual void free(void);
```

## See Also

### Configuring the Action

+ Create

Creates a new action object and configures it with your custom target object and callback method.

- SetAbortedHandler

Install a handler for the system to call when no other processes reference the action object.

