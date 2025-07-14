

- Combine
- Publishers
- Publishers.Scan
-  makeConnectable() 

Instance Method

# makeConnectable()

Creates a connectable wrapper around the publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func makeConnectable() -> Publishers.MakeConnectable
```

Available when `Failure` is `Never`.

## Return Value

A ConnectablePublisher wrapping this publisher.

## Discussion

In the following example, makeConnectable() wraps its upstream publisher (an instance of Publishers.Share) with a ConnectablePublisher. Without this, the first sink subscriber would receive all the elements from the sequence publisher and cause it to complete before the second subscriber attaches. By making the publisher connectable, the publisher doesn’t produce any elements until after the connect() call.

```
 let subject = Just("Sent")
 let pub = subject
     .share()
     .makeConnectable()
 cancellable1 = pub.sink { print ("Stream 1 received: \($0)")  }

 // For example purposes, use DispatchQueue to add a second subscriber
 // a second later, and then connect to the publisher a second after that.
 DispatchQueue.main.asyncAfter(deadline: .now() + 1) {
     self.cancellable2 = pub.sink { print ("Stream 2 received: \($0)") }
 }
 DispatchQueue.main.asyncAfter(deadline: .now() + 2) {
     self.connectable = pub.connect()
 }
 // Prints:
 // Stream 2 received: Sent
 // Stream 1 received: Sent
```

Note

The connect() operator returns a Cancellable instance that you must retain. You can also use this instance to cancel publishing.

