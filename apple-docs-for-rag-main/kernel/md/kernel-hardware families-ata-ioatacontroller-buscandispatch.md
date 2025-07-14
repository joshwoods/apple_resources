

- Kernel
- Hardware Families
- ATA
- IOATAController
-  busCanDispatch 

# busCanDispatch

answers whether the bus is in state such that the next command can be dispatched.

``` source
virtual bool busCanDispatch(
 void ); 
```

## Return Value

true - bus is free to issue commands. false - bus cannot issue commands at this time.

## See Also

### Miscellaneous

dispatchNext

Causes the command at the front of the queue to dequeue, made the current command and begin execution.

handleCommand

Called by executeCommand() to handle the client command from the workloop context.

