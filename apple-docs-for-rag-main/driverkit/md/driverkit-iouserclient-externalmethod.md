

- DriverKit
- IOUserClient
-  ExternalMethod 

Instance Method

# ExternalMethod

Receive arguments from IOKit.framework IOConnectMethod calls.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t ExternalMethod(uint64_t selector, IOUserClientMethodArguments * arguments, const IOUserClientMethodDispatch * dispatch, OSObject * target, void * reference);
```

## Parameters 

`selector`  

Selector argument to `IOConnectMethod`.

`arguments`  

Structure describing all arguments being passed to `IOConnectMethod`. See the IOUserClientMethodArguments definition.

`dispatch`  

NULL when called in the driver. The ExternalMethod implementation may be called with a non-NULL argument to check certain fields of the arguments structure before calling a target procedure specified by the dispatch structure ‘function’ field, and the ‘target’ and ‘reference’ parameters to this method. See the IOUserClientMethodDispatch definition.

`target`  

Target for the dispatch function

`reference`  

Reference constant for the dispatch function

## Return Value

kIOReturnSuccess on success. See IOReturn.h for error codes.

## Discussion

IOConnectMethod calls from the owner of the connection come here. Any argument may be passed as NULL if not passed by the caller.

## See Also

### Responding to Messages

IOUserClientMethodArguments

Arguments to pass to IOConnectMethod calls.

IOUserClientMethodDispatch

A structure that specifies how to validate the arguments passed to a client method function.

IOUserClientMethodFunction

