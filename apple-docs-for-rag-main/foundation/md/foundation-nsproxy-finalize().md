

- Foundation
- NSProxy
-  finalize() 

Instance Method

# finalize()

The garbage collector invokes this method on the receiver before disposing of the memory it uses.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func finalize()
```

## Discussion

This method behaves as described in the `NSObject` class specification under the finalize() instance method. Note that a `finalize` method must be thread-safe.

## See Also

### Related Documentation

func dealloc()

Deallocates the memory occupied by the receiver.

