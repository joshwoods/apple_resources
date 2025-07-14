

- Kernel
- Hardware Families
- FireWire
- IOFWPseudoAddressSpaceAux
-  setARxReqIntCompleteHandler 

# setARxReqIntCompleteHandler

Installs a callback to receive notification, when FWIM has completed ARxReqInt processing and no incoming packets are left in the queue.

``` source
virtual void setARxReqIntCompleteHandler(
 void *refcon,
 IOFWARxReqIntCompleteHandlerhandler ); 
```

## Parameters 

`refcon`  

Client's callback object.

`handler`  

Client callback to be invoked, at the end of interrupt processing.

## Return Value

none.

