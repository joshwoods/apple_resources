

- Combine
- Subscribers
-  Subscribers.Sink 

Class

# Subscribers.Sink

A simple subscriber that requests an unlimited number of values upon subscription.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class Sink where Failure : Error
```

## Mentioned in 

Processing Published Elements with Subscribers

## Topics

### Canceling Publication

func cancel()

Cancel the activity.

### Receiving Life Cycle Events

func receive(subscription: any Subscription)

Tells the subscriber that it has successfully subscribed to the publisher and may request items.

### Supporting Debugging

var combineIdentifier: CombineIdentifier

A unique identifier for identifying publisher streams.

var customMirror: Mirror

The custom mirror for this instance.

var description: String

A textual representation of this instance.

var playgroundDescription: Any

A custom playground description for this instance.

### Initializers

init(receiveCompletion: (Subscribers.Completion&lt;Failure>) -> Void, receiveValue: (Input) -> Void)

Initializes a sink with the provided closures.

### Instance Properties

var receiveCompletion: (Subscribers.Completion&lt;Failure>) -> Void

The closure to execute on completion.

var receiveValue: (Input) -> Void

The closure to execute on receipt of a value.

### Instance Methods

func receive(Input) -> Subscribers.Demand

Tells the subscriber that the publisher has produced an element.

func receive(completion: Subscribers.Completion&lt;Failure>)

Tells the subscriber that the publisher has completed publishing, either normally or with an error.

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

class Assign

A simple subscriber that assigns received elements to a property indicated by a key path.

