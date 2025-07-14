

- Foundation
- NSRecursiveLock
-  try() 

Instance Method

# try()

Attempts to acquire a lock, and immediately returns a Boolean value that indicates whether the attempt was successful.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func `try`() -> Bool
```

## Return Value

true if successful, otherwise false.

## See Also

### Acquiring a Lock

func lock(before: Date) -> Bool

Attempts to acquire a lock before a given date.

