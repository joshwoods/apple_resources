

- Network
- NWConnection
- NWConnection.SendCompletion
-  NWConnection.SendCompletion.contentProcessed(\_:) 

Case

# NWConnection.SendCompletion.contentProcessed(\_:)

Provide a completion handler that’s invoked when the sent data is processed by the stack.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@preconcurrency
case contentProcessed((NWError?) -> Void)
```

## See Also

### Completions

case idempotent

Mark the sent data as idempotent—data that can be sent multiple times.

