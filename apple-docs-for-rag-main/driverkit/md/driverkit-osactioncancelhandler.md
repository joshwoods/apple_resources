

- DriverKit
-  OSActionCancelHandler 

Type Alias

# OSActionCancelHandler

The block to call after the successful cancellation of the action.

DriverKitiOSiPadOSmacOS

``` source
typedef void (^)(void) OSActionCancelHandler;
```

## See Also

### Ending the Action Early

Cancel

Cancels the execution of the action’s callbacks.

Aborted

Calls the abort handler of the action object.

OSActionAbortedHandler

The block to call before aborting an action object.

