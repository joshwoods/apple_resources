

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchQueue
-  GetName 

Instance Method

# GetName

Returns the name of the queue as a C string.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
const char * GetName(void);
```

## Return Value

A C-string pointer to the queue's internal storage.

## Discussion

Returns a pointer to the queue's name. This string is valid only while the queue is retained.

## See Also

### Getting Queue Information

IODispatchQueueName

A buffer for specifying the name of a dispatch queue.

- OnQueue

Returns a Boolean value that indicates whether the current thread matches the dispatch queue's thread.

