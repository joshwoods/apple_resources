

- Kernel
- IOKit Fundamentals
- IOStream
-  sendOutputNotification 

# sendOutputNotification

Send a notification to the user client that data is available for reading on the output queue. This will result in the user's output handler being called, if they registered one.

``` source
virtual IOReturn sendOutputNotification(
 void); 
```

## Return Value

Returns kIOReturnSuccess if the notification was successfully sent.

## See Also

### Managing notification ports

getInputPort

Get the Mach port used to receive notifications from user space that a buffer has been added to the input queue.

getOutputPort

Get the Mach port used to send notifications to user space that a buffer has been added to the output queue.

setInputPort

Set the Mach port used to receive notifications from user space that a buffer has been added to the input queue.

setOutputPort

Set the Mach port used to send notifications to user space that a buffer has been added to the output queue.

