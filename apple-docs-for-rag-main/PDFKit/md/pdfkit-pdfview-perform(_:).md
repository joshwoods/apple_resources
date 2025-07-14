

- PDFKit
- PDFView
-  perform(\_:) 

Instance Method

# perform(\_:)

Performs the specified action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func perform(_ action: PDFAction)
```

## See Also

### Working with Mouse Position and Events

func areaOfInterest(forMouse: UIEvent) -> PDFAreaOfInterest

Returns the type of area the mouse cursor is over.

func areaOfInterest(for: CGPoint) -> PDFAreaOfInterest

Returns the type of area for a specific cursor location point.

struct PDFAreaOfInterest

The mouse position over PDF view areas.

func setCursorFor(PDFAreaOfInterest)

Sets the type of mouse cursor according to the type of area the mouse cursor is over.

Drag Operations

Define drag operations allowed for a view.

