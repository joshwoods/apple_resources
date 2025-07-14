

- PencilKit
-  PKDrawingReference 

Class

# PKDrawingReference

A data structure that contains the drawing information captured by a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class PKDrawingReference
```

## Overview

A PKDrawingReference object stores the user-drawn content from a PKCanvasView object. You use drawing objects to store the data associated with your user’s drawings. You can save this data with the rest of your app’s content, and you can use that saved data to create a new drawing object later. You can also generate an image based on the drawn content.

## Topics

### Creating a drawing object

init(data: Data) throws

Creates a drawing object and populates it with previously drawn content.

convenience init(strokes: [PKStroke])

Creates a drawing object with the strokes you supply.

init()

Creates an empty drawing object.

### Getting the canvas bounds

var bounds: CGRect

The smallest rectangle used to represent the content’s bounds, taking into account line widths of that content.

### Generating an image

func image(from: CGRect, scale: CGFloat) -> UIImage

Returns an image object that contains the specified portion of the drawing.

### Getting the drawing data

var strokes: [PKStroke]

An array of strokes used to represent the drawing.

func dataRepresentation() -> Data

Returns a representation of the rendered content as data.

let PKAppleDrawingTypeIdentifier: CFString

The uniform type identifier for data associated with a drawing object.

### Modifying the drawing

func applying(CGAffineTransform) -> PKDrawing

Returns a new drawing object by applying the specified transform to a copy of the current object’s contents.

func appendingStrokes([PKStroke]) -> PKDrawing

Returns a copy of the current drawing with the strokes you provide appended.

func appending(PKDrawing) -> PKDrawing

Returns a new drawing created by appending the current drawing with another drawing you provide.

### Supporting backward compatibility

var requiredContentVersion: PKContentVersion

The version of PencilKit necessary to use the drawing.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

