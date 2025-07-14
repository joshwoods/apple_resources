

- SceneKit
-  SCNLayer Deprecated

Class

# SCNLayer

A Core Animation layer that renders a SceneKit scene as its content.

macOS 10.8–10.14Deprecated

``` source
class SCNLayer
```

Deprecated

OpenGL API deprecated, please use Metal instead. (Define SCN_SILENCE_GL_DEPRECATION to silence these warnings)

## Overview

Use this class to integrate 3D content rendered by SceneKit into a user interface composed of Core Animation layers. To provide content for the layer, assign an SCNScene object to its scene property.

Most of the methods and properties you use for working with a SceneKit layer are defined by the SCNSceneRenderer protocol.

## Topics

### Specifying a Scene

var scene: SCNScene?

The scene to be displayed in the layer.

## Relationships

### Inherits From

- CAOpenGLLayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- SCNSceneRenderer
- SCNTechniqueSupport

## See Also

### Display and Interactivity

protocol SCNSceneRenderer

Methods and properties common to the SCNView, SCNLayer, and SCNRenderer classes.

protocol SCNSceneRendererDelegate

Methods your app can implement to participate in SceneKit’s animation loop or perform additional rendering.

class SCNRenderer

A renderer for displaying a SceneKit scene in an existing Metal workflow or OpenGL context.

class SCNHitTestResult

Information about the result of a scene-space or view-space search for scene elements.

