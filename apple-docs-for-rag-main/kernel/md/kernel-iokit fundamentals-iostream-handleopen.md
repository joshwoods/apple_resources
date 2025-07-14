

- Kernel
- IOKit Fundamentals
- IOStream
-  handleOpen 

# handleOpen

The handleOpen() method relies on the default IOService behavior to ensure that only one client has the stream open at a time. The shared input and output queues are created at open time.

``` source
virtual bool handleOpen(
 IOService *forClient, 
 IOOptionBits options, 
 void *arg ); 
```

## Parameters 

`options`  

`arg`  

## See Also

### Opening and closing streams

handleClose

The handleClose method destroys the shared input and output queues.

