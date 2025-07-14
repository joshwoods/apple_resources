

- DriverKit
-  IODispatchSourceCancelHandler 

Type Alias

# IODispatchSourceCancelHandler

A block to execute when a canceled dispatch source stops executing tasks.

DriverKitiOSiPadOSmacOS

``` source
typedef void (^)(void) IODispatchSourceCancelHandler;
```

## See Also

### Starting and Stopping the Interrupt Source

SetEnableWithCompletion

Enables or disables the delivery of interrupts.

Cancel

Cancels all callbacks from the event source.

