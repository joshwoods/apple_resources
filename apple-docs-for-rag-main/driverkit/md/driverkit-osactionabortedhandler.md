

- DriverKit
-  OSActionAbortedHandler 

Type Alias

# OSActionAbortedHandler

The block to call before aborting an action object.

DriverKitiOSiPadOSmacOS

``` source
typedef void (^)(void) OSActionAbortedHandler;
```

## See Also

### Ending the Action Early

Cancel

Cancels the execution of the action’s callbacks.

Aborted

Calls the abort handler of the action object.

OSActionCancelHandler

The block to call after the successful cancellation of the action.

