

- PDFKit
- PDFView
-  areaOfInterest(for:) 

Instance Method

# areaOfInterest(for:)

Returns the type of area for a specific cursor location point.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func areaOfInterest(for cursorLocation: CGPoint) -> PDFAreaOfInterest
```

**macOS**

``` source
@MainActor
func areaOfInterest(for cursorLocation: NSPoint) -> PDFAreaOfInterest
```

## See Also

### Working with Mouse Position and Events

func areaOfInterest(forMouse: UIEvent) -> PDFAreaOfInterest

Returns the type of area the mouse cursor is over.

struct PDFAreaOfInterest

The mouse position over PDF view areas.

func setCursorFor(PDFAreaOfInterest)

Sets the type of mouse cursor according to the type of area the mouse cursor is over.

func perform(PDFAction)

Performs the specified action.

Drag Operations

Define drag operations allowed for a view.

