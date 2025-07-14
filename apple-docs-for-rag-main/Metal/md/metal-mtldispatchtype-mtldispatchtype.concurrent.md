

- Metal
- MTLDispatchType
-  MTLDispatchType.concurrent 

Case

# MTLDispatchType.concurrent

Sets a command encoder to dispatch encoded commands concurrently during your pass.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
case concurrent
```

## Discussion

If you encode multiple commands that access the same resources, you’re responsible for synchronizing access to those resources. See `Controlling execution and memory barriers` for information on how to safely synchronize and access data.

## See Also

### Execution Dispatch Types

case serial

Sets a command encoder to dispatch encoded commands serially during your pass.

