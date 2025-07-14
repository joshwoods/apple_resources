

- Kernel
- Hardware Families
- ATA
- IOATAController
-  dispatchNext 

# dispatchNext

Causes the command at the front of the queue to dequeue, made the current command and begin execution.

``` source
virtual IOReturn dispatchNext(
 void ); 
```

## Return Value

noErr indicates successful dispatch.

## See Also

### Miscellaneous

busCanDispatch

answers whether the bus is in state such that the next command can be dispatched.

handleCommand

Called by executeCommand() to handle the client command from the workloop context.

