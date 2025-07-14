

- RealityKit
-  ResolvedModel3D 

Structure

# ResolvedModel3D

A view for displaying static three-dimensional models.

RealityKitSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
struct ResolvedModel3D
```

## Overview

You don’t instantiate this type directly, instead Model3D creates instances for you.

## Topics

### Instance Properties

var body: some View

The content and behavior of the view.

### Instance Methods

func resizable(Bool) -> ResolvedModel3D

Allows this model to resize itself to fit its container.

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

### SwiftUI 3D model presentation

struct Model3D

A view that asynchronously loads and displays a 3D model.

enum Model3DPhase

The current phase of the asynchronous model loading operation.

struct Model3DPlaceholderContent

A container view that presents either a 3D model or a placeholder for one.

