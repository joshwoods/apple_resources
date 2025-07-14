

- Foundation
- NSDiscardableContent
-  endContentAccess() 

Instance Method

# endContentAccess()

Called if the discardable contents are no longer being accessed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func endContentAccess()
```

**Required**

## Discussion

This method decrements the counter variable of the object, which will usually bring the value of the counter variable back down to 0, which allows the discardable contents of the object to be thrown away if necessary.

## See Also

### Accessing Content

func beginContentAccess() -> Bool

Returns a Boolean value indicating whether the discardable contents are still available and have been successfully accessed.

**Required**

