

- Kernel
- Hardware Families
- ATA
- IOATAController
-  handleCommand 

# handleCommand

Called by executeCommand() to handle the client command from the workloop context.

``` source
virtual IOReturn handleCommand(
 void *command, 
 void *param1 = 0, 
 void *param2 = 0, 
 void *param3 = 0); 
```

## Parameters 

`command`  

The command code.

`param1`  

Command parameter.

`param2`  

Command parameter.

`param3`  

Command parameter.

## Return Value

kIOReturnSuccess on success, or an error code otherwise.

## See Also

### Miscellaneous

busCanDispatch

answers whether the bus is in state such that the next command can be dispatched.

dispatchNext

Causes the command at the front of the queue to dequeue, made the current command and begin execution.

