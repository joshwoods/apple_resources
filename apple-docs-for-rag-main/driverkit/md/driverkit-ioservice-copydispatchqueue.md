

- DriverKit
- IOService
-  CopyDispatchQueue 

Instance Method

# CopyDispatchQueue

Gets the dispatch queue with the specified name from the current service.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t CopyDispatchQueue(const IODispatchQueueName name, IODispatchQueue * * queue);
```

## Parameters 

`name`  

The name you assigned to the dispatch queue. Specify `kIOServiceDefaultQueueName` to retrieve the default dispatch queue.

`queue`  

A variable to use for storing the dispatch queue. On return, this parameter contains the retained queue, or `NULL` if no queue matches the specified name. You are responsible for releasing the returned dispatch queue.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## See Also

### Configuring Additional Dispatch Queues

SetDispatchQueue

Associates a custom dispatch queue with the service and assigns the specified name to it.

