

- RealityKit
-  AccessibilityComponent 

Structure

# AccessibilityComponent

A component that stores accessibility information for an entity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS

``` source
struct AccessibilityComponent
```

## Overview

Add an `AccessibilityComponent` to entities to provide accessibility information to the system, such as the entity’s name which VoiceOver says aloud when it describes the entity.

See Improving the Accessibility of RealityKit Apps for more information.

## Topics

### Creating an accessibility component

init()

Creates a new accessibility component with default values.

### Providing accessibility information

var isAccessibilityElement: Bool

A Boolean value indicating whether the receiver is an accessibility entity that an assistive application can access.

var label: LocalizedStringResource?

A succinct label that identifies the entity, in a localized string key.

var value: LocalizedStringResource?

A localized string key that represents the current value of the entity.

### Defining traits

var traits: UIAccessibilityTraits

The combination of accessibility traits that best characterize the entity.

### Defining actions

var systemActions: AccessibilityComponent.SupportedActions

The set of supported accessibility actions.

### Specifying custom data

var customActions: [LocalizedStringResource]

An array of custom actions supported by the entity, identified by their localized string key.

var customContent: [AccessibilityComponent.CustomContent]

An array of custom content objects that deliver accessibility information.

### Identifying the next element

var customRotors: [AccessibilityComponent.RotorType]

An array of supported rotors.

### Structures

struct CustomContent

A CustomContent struct contains the accessibility strings for the labels you apply to your accessibility content.

struct SupportedActions

A custom action that can be invoked on an entity in response to specific user cues.

### Enumerations

enum RotorType

A context-sensitive event that helps VoiceOver users find the next instance of a related element.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Accessibility

Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

struct SupportedActions

A custom action that can be invoked on an entity in response to specific user cues.

struct CustomContent

A CustomContent struct contains the accessibility strings for the labels you apply to your accessibility content.

enum RotorType

A context-sensitive event that helps VoiceOver users find the next instance of a related element.

enum AccessibilityEvents

