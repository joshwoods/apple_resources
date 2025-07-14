

- RealityKit
- ARView
-  ARView.RenderCallbacks 

Structure

# ARView.RenderCallbacks

A container that holds the view’s render callbacks.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct RenderCallbacks
```

## Overview

Render callbacks are closures RealityKit calls at predefined times. You can use render callbacks to modify the results of RealityKit’s rendering. If you assign a function or closure to any of the contained callback properties, RealityKit calls that function or closure at a predefined time. Setting the postProcess property, for example, causes RealityKit to call the assigned function or closure every frame, after RealityKit renders the scene, but before it displays it.

## Topics

### Creating a callback object

init()

Creates a new object.

### Register callback closures

var prepareWithDevice: ((any MTLDevice) -> Void)?

A callback function for doing initial setup work.

var postProcess: ((ARView.PostProcessContext) -> Void)?

A callback function for implementing postprocess effects.

## See Also

### Postprocessing

Postprocessing effects

Create special rendering effects for your RealityKit scenes.

struct PostProcessContext

An object the framework uses to pass data to a postprocess callback.

