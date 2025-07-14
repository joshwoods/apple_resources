

- RealityKit
-  RealityViewContentProtocol 

Protocol

# RealityViewContentProtocol

A protocol representing the content of a reality view.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
protocol RealityViewContentProtocol
```

## Overview

Do not interface with this protocol directly. Instead, use RealityViewContent with your RealityView.

## Topics

### Managing view content

func add(Entity)

Adds an entity to this content.

func remove(Entity)

Removes an entity from this content, if present.

associatedtype Entities : EntityCollection

The type of collection used for `entities`.

**Required**

var entities: Self.Entities

A collection of RealityKit entities that this view content renders within the scene.

**Required**

### Handling subscriptions

func subscribe&lt;E>(to: E.Type, on: (any EventSource)?, (E) -> Void) -> EventSubscription

Subscribes to an event type, optionally limited to events affecting a source entity or scene.

func subscribe&lt;E>(to: E.Type, componentType: (any Component.Type)?, (E) -> Void) -> EventSubscription

Subscribes to an event type, optionally limited to a specific component type for component events.

func subscribe&lt;E>(to: E.Type, on: (any EventSource)?, componentType: (any Component.Type)?, (E) -> Void) -> EventSubscription

Subscribes to an event type, optionally limited to events affecting a source entity or scene, or a specific component type for component events.

**Required**

## Relationships

### Conforming Types

- RealityViewCameraContent
- RealityViewContent

## See Also

### SwiftUI scene presentation

struct RealityView

A view that contains RealityKit content.

struct RealityViewContent

The content of a visionOS reality view.

struct RealityViewCameraContent

The content of a reality view that is displayed through a camera.

struct RealityViewDefaultPlaceholder

A view that represents the default placeholder for a RealityView.

struct RealityViewEntityCollection

A collection of entities in a RealityView.

protocol EntityCollection

An ordered, mutable collection of entities.

