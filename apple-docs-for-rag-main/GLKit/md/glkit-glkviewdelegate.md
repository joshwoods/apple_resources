

- GLKit
-  GLKViewDelegate 

Protocol

# GLKViewDelegate

Drawing callback methods for use with a GLKView object.

iOS 5.0+iPadOS 5.0+tvOS 9.0+

``` source
protocol GLKViewDelegate : NSObjectProtocol
```

## Overview

An object that implements the GLKViewDelegate protocol can be set as a GLKView object’s delegate. A delegate allows your application to provide a drawing method to a GLKView object without subclassing the GLKView class.

## Topics

### Drawing the View’s Contents

func glkView(GLKView, drawIn: CGRect)

Draws the view’s contents.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- GLKViewController

## See Also

### OpenGL ES View Rendering

class GLKView

A default implementation for views that draw their content using OpenGL ES.

Deprecated

class GLKViewController

A view controller that manages an OpenGL ES rendering loop.

Deprecated

protocol GLKViewControllerDelegate

Rendering loop callback methods for use with a GLKViewController object.

