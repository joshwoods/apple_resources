

- DriverKit
- IOUserClient
-  AsyncCompletion 

Instance Method

# AsyncCompletion

Send asynchronous arguments to a completion supplied by ExternalMethod().

DriverKitiOSiPadOSmacOS

``` source
void AsyncCompletion(OSAction * action, IOReturn status, const IOUserClientAsyncArgumentsArray asyncData, uint32_t asyncDataCount);
```

## Parameters 

`action`  

OSAction passed to IOExternalMethod().

`status`  

An IOReturn status value to be sent.

`asyncData`  

An array of scalar data to be sent.

`asyncDataCount`  

Count of valid data in asyncData.

## Discussion

IOConnectAsyncMethod calls from the owner of the connection come will pass an OSAction instance. To deliver the asynchronous results the driver calls AsyncCompletion().

## See Also

### Communicating with the Client

KernelCompletion

IOUserClientAsyncArgumentsArray

Arguments Array Maximum

IOUserClientAsyncReferenceArray

Reference Array Maximum

