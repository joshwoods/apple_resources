

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IONotifier
-  remove 

# remove

Removes the notification request and releases it.

``` source
virtual void remove() = 0; 
```

## Overview

Removes the notification request and release it. Since creating an IONotifier instance will leave it with a retain count of one, creating an IONotifier and then removing it will destroy it. This method is synchronous with any handler invocations, so when this method returns its guaranteed the handler will not be in entered.

## See Also

### Miscellaneous

disable

Disables the notification request.

enable

Sets the enable state of the notification request.

