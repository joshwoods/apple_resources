

- RealityKit
-  SceneEvents 

Enumeration

# SceneEvents

Events the scene invokes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum SceneEvents
```

## Overview

For more information on subscribing to scene events, see `RealityKit/Scene/Event`.

## Topics

### Detecting scene-level updates

struct Update

An event invoked once per frame interval that you can use to execute custom logic for each frame.

struct AnchoredStateChanged

An event invoked when the anchored state of an anchoring entity changes.

### Detecting scene hierarchy changes

struct DidAddEntity

Raised after an entity is added to the scene.

struct DidReparentEntity

Raised after an entity has been reparented within the same scene.

struct WillRemoveEntity

Raised before an entity is removed from the scene.

struct DidActivateEntity

Raised after an entity becomes active.

struct WillDeactivateEntity

Raised before an entity becomes inactive.

## See Also

### Core event types

protocol Event

A type that can be sent as an event.

protocol EventSource

A type on which events can be published and subscribed.

struct EventSubscription

A subscription to an event.

enum ComponentEvents

Provides the events related to components.

