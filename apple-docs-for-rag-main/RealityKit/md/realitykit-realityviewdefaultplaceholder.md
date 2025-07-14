

- RealityKit
-  RealityViewDefaultPlaceholder 

Structure

# RealityViewDefaultPlaceholder

A view that represents the default placeholder for a RealityView.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
struct RealityViewDefaultPlaceholder
```

## Overview

You don’t directly create instances of this type because RealityView creates them for you.

## Topics

### Instance Properties

var body: some View

The content and behavior of the view.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### SwiftUI scene presentation

struct RealityView

A view that contains RealityKit content.

struct RealityViewContent

The content of a visionOS reality view.

struct RealityViewCameraContent

The content of a reality view that is displayed through a camera.

protocol RealityViewContentProtocol

A protocol representing the content of a reality view.

struct RealityViewEntityCollection

A collection of entities in a RealityView.

protocol EntityCollection

An ordered, mutable collection of entities.

