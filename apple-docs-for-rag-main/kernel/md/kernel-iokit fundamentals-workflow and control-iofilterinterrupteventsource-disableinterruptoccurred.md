

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOFilterInterruptEventSource
-  disableInterruptOccurred 

# disableInterruptOccurred

Override \$link IOInterruptEventSource::disableInterruptOccurred to make a filter callout.

``` source
virtual void disableInterruptOccurred(
 void *self,
 IOService *prov,
 int ind); 
```

## See Also

### Miscellaneous

filterInterruptEventSource

Factor method to create and initialise an IOFilterInterruptEventSource. See \$link init.

getFilterAction

Get'ter for filterAction variable.

init

Primary initialiser for the IOFilterInterruptEventSource class.

normalInterruptOccurred

Override \$link IOInterruptEventSource::normalInterruptOccured to make a filter callout.

signalInterrupt

Cause the work loop to schedule the action.

