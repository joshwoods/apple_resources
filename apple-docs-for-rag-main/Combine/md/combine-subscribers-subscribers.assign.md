

- Combine
- Subscribers
-  Subscribers.Assign 

Class

# Subscribers.Assign

A simple subscriber that assigns received elements to a property indicated by a key path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class Assign
```

## Mentioned in 

Processing Published Elements with Subscribers

## Topics

### Declaring Subscriber Topography

typealias Failure

The kind of errors this subscriber might receive.

### Creating an Assign Subscriber

init(object: Root, keyPath: ReferenceWritableKeyPath&lt;Root, Input>)

Creates a subscriber to assign the value of a property indicated by a key path.

### Declaring Publisher Topography

typealias Failure

The kind of errors this subscriber might receive.

### Inspecting the Assigned Property

var object: Root?

The object that contains the property to assign.

let keyPath: ReferenceWritableKeyPath&lt;Root, Input>

The key path that indicates the property to assign.

### Instance Properties

var customMirror: Mirror

A mirror that reflects the subscriber.

var description: String

A textual representation of this subscriber.

var playgroundDescription: Any

A custom playground description for this subscriber.

### Instance Methods

func cancel()

Cancel the activity.

func receive(Input) -> Subscribers.Demand

Tells the subscriber that the publisher has produced an element.

func receive(completion: Subscribers.Completion&lt;Never>)

Tells the subscriber that the publisher has completed publishing, either normally or with an error.

func receive(subscription: any Subscription)

Tells the subscriber that it has successfully subscribed to the publisher and may request items.

### Default Implementations

Cancellable Implementations

CustomCombineIdentifierConvertible Implementations

Subscriber Implementations

## Relationships

### Conforms To

- Cancellable
- CustomCombineIdentifierConvertible
- CustomPlaygroundDisplayConvertible
- CustomReflectable
- CustomStringConvertible
- Subscriber

## See Also

### Using Convenience Subscribers

class Sink

A simple subscriber that requests an unlimited number of values upon subscription.

