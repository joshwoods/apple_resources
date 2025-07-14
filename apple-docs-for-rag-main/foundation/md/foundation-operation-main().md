

- Foundation
- Operation
-  main() 

Instance Method

# main()

Performs the receiver’s non-concurrent task.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func main()
```

## Discussion

The default implementation of this method does nothing. You should override this method to perform the desired task. In your implementation, do not invoke `super`. This method will automatically execute within an autorelease pool provided by `NSOperation`, so you do not need to create your own autorelease pool block in your implementation.

If you are implementing a concurrent operation, you are not required to override this method but may do so if you plan to call it from your custom start() method.

## See Also

### Executing the Operation

func start()

Begins the execution of the operation.

var completionBlock: (() -> Void)?

The block to execute after the operation’s main task is completed.

