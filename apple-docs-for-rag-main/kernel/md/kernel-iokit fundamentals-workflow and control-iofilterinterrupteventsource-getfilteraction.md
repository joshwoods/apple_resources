

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOFilterInterruptEventSource
-  getFilterAction 

# getFilterAction

Get'ter for filterAction variable.

``` source
virtual Filter getFilterAction() const; 
```

## Return Value

value of filterAction.

## See Also

### Miscellaneous

disableInterruptOccurred

Override \$link IOInterruptEventSource::disableInterruptOccurred to make a filter callout.

filterInterruptEventSource

Factor method to create and initialise an IOFilterInterruptEventSource. See \$link init.

init

Primary initialiser for the IOFilterInterruptEventSource class.

normalInterruptOccurred

Override \$link IOInterruptEventSource::normalInterruptOccured to make a filter callout.

signalInterrupt

Cause the work loop to schedule the action.

