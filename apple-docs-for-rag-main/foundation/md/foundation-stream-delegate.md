

- Foundation
- Stream
-  delegate 

Instance Property

# delegate

Sets the receiver’s delegate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var delegate: (any StreamDelegate)? { get set }
```

## Parameters 

`delegate`  

The delegate for the receiver.

## Discussion

By default, a stream is its own delegate, and subclasses of `NSInputStream` and `NSOutputStream` must maintain this contract. If you override this method in a subclass, passing `nil` must restore the receiver as its own delegate. Delegates are not retained.

To learn about delegates and delegation, read “Delegation” in Cocoa Fundamentals Guide.

## See Also

### Configuring Streams

func property(forKey: Stream.PropertyKey) -> Any?

Returns the receiver’s property for a given key.

func setProperty(Any?, forKey: Stream.PropertyKey) -> Bool

Attempts to set the value of a given property of the receiver and returns a Boolean value that indicates whether the value is accepted by the receiver.

