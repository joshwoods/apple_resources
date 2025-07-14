

- Kernel
- IOKit Fundamentals
- IOStream
-  setOutputPort 

# setOutputPort

Set the Mach port used to send notifications to user space that a buffer has been added to the output queue.

``` source
virtual IOReturn setOutputPort(
 mach_port_tport); 
```

## Parameters 

`port`  

## See Also

### Managing notification ports

getInputPort

Get the Mach port used to receive notifications from user space that a buffer has been added to the input queue.

getOutputPort

Get the Mach port used to send notifications to user space that a buffer has been added to the output queue.

sendOutputNotification

Send a notification to the user client that data is available for reading on the output queue. This will result in the user's output handler being called, if they registered one.

setInputPort

Set the Mach port used to receive notifications from user space that a buffer has been added to the input queue.

