

- DriverKit
- OSAction
-  Aborted 

Instance Method

# Aborted

Calls the abort handler of the action object.

DriverKitiOSiPadOSmacOS

``` source
void Aborted();
```

## Discussion

Don’t call this method directly. The system calls it when no other objects reference the action object.

## See Also

### Ending the Action Early

Cancel

Cancels the execution of the action’s callbacks.

OSActionAbortedHandler

The block to call before aborting an action object.

OSActionCancelHandler

The block to call after the successful cancellation of the action.

