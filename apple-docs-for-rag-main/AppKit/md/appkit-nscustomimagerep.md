

- AppKit
-  NSCustomImageRep 

Class

# NSCustomImageRep

An object that uses a delegate object to render an image from a custom format.

macOS

``` source
class NSCustomImageRep
```

## Overview

When called upon to produce an image, an NSCustomImageRep sends a message to its delegate to do the actual drawing. You can use this class to support custom image formats without going to the trouble of subclassing NSImageRep directly.

## Topics

### Creating Representations of Images in Custom Formats

init(draw: Selector, delegate: Any)

Returns a representation of an image initialized with the specified delegate information.

init(size: NSSize, flipped: Bool, drawingHandler: (NSRect) -> Bool)

Initializes a representation of an image of the specified size and flipped status, using a block to draw its content.

### Getting Drawing Handlers

var drawingHandler: ((NSRect) -> Bool)?

The destination rectangle of the drawing handler block.

### Getting Information About Images

var delegate: AnyObject?

The delegate object that renders the image for the image representation.

var drawSelector: Selector?

The selector for the delegate’s drawing method.

## Relationships

### Inherits From

- NSImageRep

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

