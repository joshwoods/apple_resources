

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchQueue
-  OnQueue 

Instance Method

# OnQueue

Returns a Boolean value that indicates whether the current thread matches the dispatch queue's thread.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
bool OnQueue(void);
```

## Return Value

`true` if the current thread is the same thread that the dispatch queue is using to execute its task.

## Discussion

Use this method to determine if your code is running on the same thread as the current dispatch queue.

## See Also

### Getting Queue Information

IODispatchQueueName

A buffer for specifying the name of a dispatch queue.

- GetName

Returns the name of the queue as a C string.

