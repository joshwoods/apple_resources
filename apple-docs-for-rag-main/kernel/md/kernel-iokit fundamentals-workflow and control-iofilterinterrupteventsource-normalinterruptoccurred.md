

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOFilterInterruptEventSource
-  normalInterruptOccurred 

# normalInterruptOccurred

Override \$link IOInterruptEventSource::normalInterruptOccured to make a filter callout.

``` source
virtual void normalInterruptOccurred(
 void *self,
 IOService *prov,
 int ind); 
```

## See Also

### Miscellaneous

disableInterruptOccurred

Override \$link IOInterruptEventSource::disableInterruptOccurred to make a filter callout.

filterInterruptEventSource

Factor method to create and initialise an IOFilterInterruptEventSource. See \$link init.

getFilterAction

Get'ter for filterAction variable.

init

Primary initialiser for the IOFilterInterruptEventSource class.

signalInterrupt

Cause the work loop to schedule the action.

