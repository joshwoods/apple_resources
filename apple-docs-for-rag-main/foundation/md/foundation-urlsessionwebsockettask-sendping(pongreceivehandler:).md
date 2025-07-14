

- Foundation
- URLSessionWebSocketTask
-  sendPing(pongReceiveHandler:) 

Instance Method

# sendPing(pongReceiveHandler:)

Sends a ping frame from the client side, with a closure to receive the pong from the server endpoint.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sendPing(pongReceiveHandler: @escaping ((any Error)?) -> Void)
```

## Parameters 

`pongReceiveHandler`  

A closure called by the task when it receives the pong from the server. The block/closure receives an NSError that indicates a lost connection or other problem, or `nil` if no error occurred.

## Discussion

When sending multiple pings, the task always calls `pongReceiveHandler` in the order it sent the pings.

