

- Kernel
- IOKit Fundamentals
- Data Types
- OSAction
-  GetReference 

Instance Method

# GetReference

Returns a pointer to any additional memory allocated by the action object on your behalf.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
void * GetReference(void);
```

## Return Value

A pointer to the additional storage you requested at creation time. This method returns `NULL` if you passed `0` to the `referenceSize` parameter of the Create method. It also returns `NULL` if the action object doesn't belong to the current process.

## Discussion

The action object zero-initializes the memory it allocates. Only the process that owns the action object may access the memory.

