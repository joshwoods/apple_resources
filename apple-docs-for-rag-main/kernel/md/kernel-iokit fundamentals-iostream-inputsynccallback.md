

- Kernel
- IOKit Fundamentals
- IOStream
-  inputSyncCallback 

# inputSyncCallback

Input callback function to be implemented by a subclass.

``` source
virtual void inputSyncCallback(
 UInt32token ); 
```

## Parameters 

`token`  

A 32-bit token value that can be used by convention to communicate from user space to the stream. The semantics of this value are defined by the IOStream subclass.

## Overview

The inputSyncCallback() method is called as a result of a fast trap from user space. It is called on the same thread as the user request, so no context switch is necessary.

## See Also

### Managing notifications

inputCallback

Input callback function to be implemented by a subclass;

