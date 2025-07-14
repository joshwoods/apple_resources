

- Metal
-  MTLDrawable 

Protocol

# MTLDrawable

A displayable resource that can be rendered or written to.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLDrawable : NSObjectProtocol
```

## Mentioned in 

Adjusting for GPU Memory Bandwidth Tradeoffs

## Overview

Objects that implement this protocol are connected both to the Metal framework and an underlying display system (such as Core Animation) that’s capable of showing content onscreen. You use drawable objects when you want to render images using Metal and present them onscreen.

Don’t implement this protocol yourself; instead, see CAMetalLayer, for a class that can create and manage drawable objects for you.

## Topics

### Identifying the Drawable

var drawableID: Int

A positive integer that identifies the drawable.

**Required**

### Presenting the Drawable

func present()

Presents the drawable onscreen as soon as possible.

**Required**

func present(afterMinimumDuration: CFTimeInterval)

Presents the drawable onscreen as soon as possible after a previous drawable is visible for the specified duration.

**Required**

func present(at: CFTimeInterval)

Presents the drawable onscreen at a specific host time.

**Required**

### Getting Presentation Information

func addPresentedHandler(MTLDrawablePresentedHandler)

Registers a block of code to be called immediately after the drawable is presented.

**Required**

var presentedTime: CFTimeInterval

The host time, in seconds, when the drawable was displayed onscreen.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Render Pass Outputs

typealias MTLDrawablePresentedHandler

A block of code invoked after a drawable is presented.

