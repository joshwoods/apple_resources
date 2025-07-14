

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IONotifier
-  disable 

# disable

Disables the notification request.

``` source
virtual bool disable() = 0; 
```

## Return Value

Returns the previous enable state of the IONotifier.

## Overview

Disables the notification request. This method is synchronous with any handler invocations, so when this method returns its guaranteed the handler will not be in entered.

## See Also

### Miscellaneous

enable

Sets the enable state of the notification request.

remove

Removes the notification request and releases it.

