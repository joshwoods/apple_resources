

- DriverKit
- IOInterruptDispatchSource
-  InterruptOccurred 

Instance Method

# InterruptOccurred

Executes custom code when an interrupt occurs.

DriverKitiOSiPadOSmacOS

``` source
void InterruptOccurred(OSAction * action, uint64_t count, uint64_t time);
```

## Parameters 

`action`  

The action object that handles the interrupt event.

`count`  

The number of interrupts that occurred.

`time`  

The time at which the interrupt occurred. The system collects this value using the mach_absolute_time function.

## Discussion

Use this method as a prototype for declaring your own custom interrupt handlers. When declaring your method, use the TYPE macro to indicate that your method has the same parameters and return value as this method.

Use the implementation of your method to respond to any interrupts that occurred.

## See Also

### Declaring Actions

CheckForWork

Checks for events to handle.

IOInterruptDispatchSourcePayload

A private structure for an interrupt dispatch source.

