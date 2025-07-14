

- Foundation
- NSDistributedLock
-  try() 

Instance Method

# try()

Attempts to acquire the receiver and immediately returns a Boolean value that indicates whether the attempt was successful.

Mac Catalyst 13.0+macOS 10.0+

``` source
func `try`() -> Bool
```

## Return Value

true if the attempt to acquire the receiver was successful, otherwise false.

## Discussion

Raises `NSGenericException` if a file-system error occurs.

## See Also

### Related Documentation

func unlock()

Relinquishes the receiver.

