

- PencilKit
-  PKDrawing 

Structure

# PKDrawing

A structure representing the drawing information captured by a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
struct PKDrawing
```

## Mentioned in 

Supporting backward compatibility for ink types

## Overview

A PKDrawing object stores the user-drawn content from a PKCanvasView object. You use drawing objects to store the data associated with your user’s drawings. You can save this data with the rest of your app’s content, and you can use that saved data to create a new drawing object later. You can also generate an image based on the drawn content that you can copy to the pasteboard, save to disk, or share.

## Topics

### Creating a drawing object

init&lt;S>(strokes: S)

Creates a drawing object and populates it with a sequence of strokes the user provides.

init(data: Data) throws

Creates a drawing object and populates it with previously drawn content.

init()

Creates an empty drawing object.

### Getting the canvas bounds

var bounds: CGRect

The smallest rectangle used to represent the content’s bounds, taking into account line widths of that content.

### Generating an image

func image(from: CGRect, scale: CGFloat) -> UIImage

Returns an image object that contains the specified portion of the drawing.

func image(from: CGRect, scale: CGFloat) -> NSImage

Returns an image object that contains the specified portion of the drawing.

### Getting the drawing data

var strokes: [PKStroke]

The array of strokes that make up the drawing.

func dataRepresentation() -> Data

Returns a raw data representation of the rendered content.

let PKAppleDrawingTypeIdentifier: CFString

The uniform type identifier for data associated with a drawing object.

### Modifying the drawing

func transform(using: CGAffineTransform)

Applies the specified transform to the contents of this drawing.

func transformed(using: CGAffineTransform) -> PKDrawing

Applies the specified transform and returns a new drawing.

func append(PKDrawing)

Appends the contents of the specified drawing object to an existing drawing object that you provide.

func appending(PKDrawing) -> PKDrawing

Returns a new drawing created by appending the current drawing with another drawing you provide.

### Supporting backward compatibility

var requiredContentVersion: PKContentVersion

The version of PencilKit necessary to use the drawing.

### Using reference types

class PKDrawingReference

A data structure that contains the drawing information captured by a canvas view.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable

## See Also

### Canvas

Drawing with PencilKit

Add expressive, low-latency drawing to your app using PencilKit.

Customizing Scribble with Interactions

Enable writing on a non-text-input view by adding interactions.

Inspecting, Modifying, and Constructing PencilKit Drawings

Score users’ ability to match PencilKit drawings generated from text, by accessing the strokes and points inside PencilKit drawings.

class PKCanvasView

A view that captures Apple Pencil input and displays the rendered results in an iOS app.

struct PKStroke

A structure that represents the paths, boundaries, and other properties of a stroke drawn on a canvas.

struct PKStrokePath

A structure that captures the components of a stroke and provides methods to find and interpolate points along the stroke’s path.

struct PKStrokePoint

A structure that represents the properties of a specific point along a stroke’s path.

struct PKInk

A structure that represents an ink that specifies its type, color, and width.

