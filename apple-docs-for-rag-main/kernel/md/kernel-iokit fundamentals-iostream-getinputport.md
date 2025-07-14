

- Kernel
- IOKit Fundamentals
- IOStream
-  getInputPort 

# getInputPort

Get the Mach port used to receive notifications from user space that a buffer has been added to the input queue.

``` source
virtual mach_port_t getInputPort(
 void); 
```

## See Also

### Managing notification ports

getOutputPort

Get the Mach port used to send notifications to user space that a buffer has been added to the output queue.

sendOutputNotification

Send a notification to the user client that data is available for reading on the output queue. This will result in the user's output handler being called, if they registered one.

setInputPort

Set the Mach port used to receive notifications from user space that a buffer has been added to the input queue.

setOutputPort

Set the Mach port used to send notifications to user space that a buffer has been added to the output queue.

