

- DeveloperToolsSupport
-  PreviewCameraBuilder 

Structure

# PreviewCameraBuilder

A builder type that composes a collection of cameras for previewing a view in a 3D scene.

visionOS 1.0+

``` source
@resultBuilder
struct PreviewCameraBuilder
```

## Overview

You implicitly use a preview camera builder when you define a list of PreviewCamera instances for a preview macro:

```
#Preview {
    CircleImage()
} cameras: {
    PreviewCamera(from: .top, name: "Top")
    PreviewCamera(from: .leading, name: "Leading")
    PreviewCamera(from: .front, name: "Front")
}
```

## Topics

### Type Methods

static func buildArray([[PreviewCamera]]) -> [PreviewCamera]

Builds a partial result from an array of partial results.

static func buildExpression(PreviewCamera) -> [PreviewCamera]

Builds a partial result from a single camera.

static func buildExpression([PreviewCamera]) -> [PreviewCamera]

Builds a partial result from an array of cameras.

static func buildPartialBlock(accumulated: [PreviewCamera], next: [PreviewCamera]) -> [PreviewCamera]

Combines an accumulated component with a new component.

static func buildPartialBlock(first: [PreviewCamera]) -> [PreviewCamera]

Builds a partial result component from the first component.

## See Also

### Camera Management

struct PreviewCamera

A camera that defines a viewpoint in a preview.

