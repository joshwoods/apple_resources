

- Kernel
- IOKit Fundamentals
- IOStream
-  inputCallback 

# inputCallback

Input callback function to be implemented by a subclass;

``` source
virtual void inputCallback(
 UInt32token ); 
```

## Parameters 

`token`  

A 32-bit token value that can be used by convention to communicate from user space to the stream. The semantics of this value are defined by the IOStream subclass.

## Overview

The inputCallback() method is called as a result of a fast trap from user space. It is called on the same thread as the user request, but the subclass should implement this call as a notification sent to a workloop so that the request is asynchronous.

## See Also

### Managing notifications

inputSyncCallback

Input callback function to be implemented by a subclass.

