

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOFilterInterruptEventSource
-  signalInterrupt 

# signalInterrupt

Cause the work loop to schedule the action.

``` source
virtual void signalInterrupt(); 
```

## Overview

Cause the work loop to schedule the interrupt action even if the filter routine returns 'false'. Note well the interrupting condition MUST be cleared from the hardware otherwise an infinite process interrupt loop will occur. Use this function when SoftDMA is desired. See \$link IOFilterInterruptSource::Filter

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

normalInterruptOccurred

Override \$link IOInterruptEventSource::normalInterruptOccured to make a filter callout.

