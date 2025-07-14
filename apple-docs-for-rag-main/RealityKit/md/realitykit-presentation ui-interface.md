

- RealityKit
-  Presentation UI 

API Collection

# Presentation UI

Control your app’s content and how people can interact with it.

## Overview

RealityKit provides controls that enable interactions specific to each platform and context. For example, you can allow someone to interact with an entity that already has a CollisionComponent by adding the InputTargetComponent component. A RealityKit entity can visibly change when someone looks directly at it with a HoverEffectComponent component. Additionally, you can manage an entity’s accessibility information with AccessibilityComponent.

## Topics

### Direct and indirect gestures

Transforming RealityKit entities using gestures

Build a RealityKit component to support standard visionOS gestures on any entity.

struct InputTargetComponent

A component that gives an entity the ability to receive system input.

struct EntityTargetValue

A value containing an original gesture value along with a targeted entity.

### Accessibility

Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

struct AccessibilityComponent

A component that stores accessibility information for an entity.

struct SupportedActions

A custom action that can be invoked on an entity in response to specific user cues.

struct CustomContent

A CustomContent struct contains the accessibility strings for the labels you apply to your accessibility content.

enum RotorType

A context-sensitive event that helps VoiceOver users find the next instance of a related element.

enum AccessibilityEvents

### Visual adjustments

struct HoverEffectComponent

A component that applies a visual effect to a hierarchy of entities when a person looks at or selects an entity.

struct BillboardComponent

A component that orients an entity instance so that it continuously points toward the active camera.

### UIKit and AppKit gestures

struct EntityGestures

The set of possible entity gesture recognizers.

class EntityRotationGestureRecognizer

A gesture recognizer that uses rotation gestures involving two touches to rotate a given entity.

class EntityScaleGestureRecognizer

A gesture recognizer that uses a pinch gesture to scale or zoom an entity.

class EntityTranslationGestureRecognizer

A gesture recognizer that uses a pan gesture to move an entity.

protocol EntityGestureRecognizer

A gesture recognizer that works on entities.

## See Also

### Presentation

Views and attachments

Bring RealityKit content into your app with views and renderers.

