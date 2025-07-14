

- MetalKit
-  MTKViewDelegate 

Protocol

# MTKViewDelegate

Methods for responding to a MetalKit view’s drawing and resizing events.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol MTKViewDelegate : NSObjectProtocol
```

## Overview

You can set an object that implements the MTKViewDelegate protocol as a MTKView object’s delegate. Use a delegate to provide a drawing method to a MTKView object and respond to rendering events without subclassing the MTKView class.

## Topics

### Changing the View’s Layout

func mtkView(MTKView, drawableSizeWillChange: CGSize)

Updates the view’s contents upon receiving a change in layout, resolution, or size.

**Required**

### Drawing the View’s Contents

func draw(in: MTKView)

Draws the view’s contents.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### View Management

class MTKView

A specialized view that creates, configures, and displays Metal objects.

