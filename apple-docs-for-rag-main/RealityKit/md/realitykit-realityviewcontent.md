

- RealityKit
-  RealityViewContent 

Structure

# RealityViewContent

The content of a visionOS reality view.

RealityKitSwiftUIvisionOS 1.0+

``` source
struct RealityViewContent
```

## Overview

Add content that you want your visionOS app to display to a `RealityViewContent`.

You can use `RealityViewContent` to add and remove entities, subscribe to RealityKit events, and perform coordinate conversions between RealityKit entity space and a SwiftUI View’s coordinate space.

## Topics

### Structures

struct Body

The default view contents of a reality view, using reality view content.

### Instance Properties

var entities: RealityViewEntityCollection

A collection of RealityKit entities that this view content renders within the scene.

### Instance Methods

func subscribe&lt;E>(to: E.Type, on: (any EventSource)?, componentType: (any Component.Type)?, (E) -> Void) -> EventSubscription

Subscribes to an event type, optionally limited to events affecting a source entity or scene, or a specific component type for component events.

### Type Aliases

typealias Entities

The type of collection used for `entities`.

### Default Implementations

RealityCoordinateSpaceConverting Implementations

RealityViewContentProtocol Implementations

## Relationships

### Conforms To

- Copyable
- RealityCoordinateSpace
- RealityCoordinateSpaceConverting
- RealityViewContentProtocol

## See Also

### SwiftUI scene presentation

struct RealityView

A view that contains RealityKit content.

struct RealityViewCameraContent

The content of a reality view that is displayed through a camera.

protocol RealityViewContentProtocol

A protocol representing the content of a reality view.

struct RealityViewDefaultPlaceholder

A view that represents the default placeholder for a RealityView.

struct RealityViewEntityCollection

A collection of entities in a RealityView.

protocol EntityCollection

An ordered, mutable collection of entities.

