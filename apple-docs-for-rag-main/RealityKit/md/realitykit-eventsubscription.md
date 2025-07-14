

- RealityKit
-  EventSubscription 

Structure

# EventSubscription

A subscription to an event.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct EventSubscription
```

## Topics

### Instance Methods

func cancel()

Cancels the event subscription.

func subscribe(to: Scene)

## See Also

### Core event types

protocol Event

A type that can be sent as an event.

protocol EventSource

A type on which events can be published and subscribed.

enum SceneEvents

Events the scene invokes.

enum ComponentEvents

Provides the events related to components.

