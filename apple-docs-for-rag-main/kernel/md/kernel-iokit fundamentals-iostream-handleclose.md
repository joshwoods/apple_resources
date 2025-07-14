

- Kernel
- IOKit Fundamentals
- IOStream
-  handleClose 

# handleClose

The handleClose method destroys the shared input and output queues.

``` source
virtual void handleClose(
 IOService *forClient, 
 IOOptionBits options ); 
```

## Parameters 

`options`  

## See Also

### Opening and closing streams

handleOpen

The handleOpen() method relies on the default IOService behavior to ensure that only one client has the stream open at a time. The shared input and output queues are created at open time.

