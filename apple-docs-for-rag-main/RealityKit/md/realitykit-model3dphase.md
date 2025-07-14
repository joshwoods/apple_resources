

- RealityKit
-  Model3DPhase 

Enumeration

# Model3DPhase

The current phase of the asynchronous model loading operation.

RealityKitSwiftUIvisionOS 1.0+

``` source
enum Model3DPhase
```

## Overview

When you create a Model3D instance with the init(url:transaction:content:) or `Model3D/init(named:transaction:content:)` initializers, you define the appearance of the view using a `content` closure. Model3D calls the closure with a phase value at different points during the load operation to indicate the current state. Use the phase to decide what to display. For example, you can display the loaded model if it exists, a view that indicates an error, or a placeholder:

```
let url = URL(string: "https://example.com/robot.usdz")!
Model3D(url: url) { phase in
    if let model = phase.model {
        model // Displays the loaded model.
    } else if phase.error != nil {
        Color.red // Indicates an error.
    } else {
        ProgressView()
    }
}
```

## Topics

### Accessing the model

var model: ResolvedModel3D?

The loaded model, if any.

var error: (any Error)?

The error that occurred when attempting to load a model, if any.

### Obtaining the result

case empty

No model is loaded.

case success(ResolvedModel3D)

A model has succesfully loaded.

case failure(any Error)

An model failed to load with an error.

## See Also

### SwiftUI 3D model presentation

struct Model3D

A view that asynchronously loads and displays a 3D model.

struct ResolvedModel3D

A view for displaying static three-dimensional models.

struct Model3DPlaceholderContent

A container view that presents either a 3D model or a placeholder for one.

