

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IONotifier
-  enable 

# enable

Sets the enable state of the notification request.

``` source
virtual void enable(
 boolwas ) = 0; 
```

## Parameters 

`was`  

The enable state of the notifier to restore.

## Overview

Restores the enable state of the notification request, given the previous state passed in.

## See Also

### Miscellaneous

disable

Disables the notification request.

remove

Removes the notification request and releases it.

