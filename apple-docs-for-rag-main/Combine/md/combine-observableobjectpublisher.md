

- Combine
-  ObservableObjectPublisher 

Class

# ObservableObjectPublisher

A publisher that publishes changes from observable objects.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class ObservableObjectPublisher
```

## Topics

### Creating an Observable Object Publisher

init()

Creates an observable object publisher instance.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Delivering Elements to Subscribers

func send()

Sends the changed value to the downstream subscriber.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Observable Objects

protocol ObservableObject

A type of object with a publisher that emits before the object has changed.

