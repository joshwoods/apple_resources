

- Network
- NWConnection
- NWConnection.SendCompletion
-  NWConnection.SendCompletion.idempotent 

Case

# NWConnection.SendCompletion.idempotent

Mark the sent data as idempotent—data that can be sent multiple times.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case idempotent
```

## See Also

### Completions

case contentProcessed((NWError?) -> Void)

Provide a completion handler that’s invoked when the sent data is processed by the stack.

