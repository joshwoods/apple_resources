

- Combine
- PassthroughSubject
-  send() 

Instance Method

# send()

Sends a void value to the subscriber.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func send()
```

Available when `Output` is `()`.

## Discussion

Use `Void` inputs and outputs when you want to signal that an event has occurred, but don’t need to send the event itself.

## See Also

### Delivering Elements to Subscribers

func send(Output)

Sends a value to the subscriber.

