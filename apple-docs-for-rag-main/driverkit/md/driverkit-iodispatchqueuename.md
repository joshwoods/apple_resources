

- DriverKit
-  IODispatchQueueName 

Type Alias

# IODispatchQueueName

A buffer for specifying the name of a dispatch queue.

DriverKitiOSiPadOSmacOS

``` source
typedef char[256] IODispatchQueueName;
```

## See Also

### Getting Queue Information

GetName

Returns the name of the queue as a C string.

OnQueue

Returns a Boolean value that indicates whether the current thread matches the dispatch queue’s thread.

