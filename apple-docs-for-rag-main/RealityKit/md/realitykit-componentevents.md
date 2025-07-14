

- RealityKit
-  ComponentEvents 

Enumeration

# ComponentEvents

Provides the events related to components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum ComponentEvents
```

## Overview

For more information on subscribing to scene events, see `RealityKit/Scene/Event`.

## Topics

### Detecting component changes

struct DidAdd

Event raised after a component has been added to an entity,

struct DidChange

Event raised after a component has been modified.

struct WillRemove

Event raised before a component is removed from an entity.

### Detecting component activations

struct DidActivate

Event raised after a component has been activated.

struct WillDeactivate

Event raised before a component is deactivated.

## See Also

### Core event types

protocol Event

A type that can be sent as an event.

protocol EventSource

A type on which events can be published and subscribed.

struct EventSubscription

A subscription to an event.

enum SceneEvents

Events the scene invokes.

