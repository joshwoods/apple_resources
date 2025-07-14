

- PDFKit
- PDFView
-  areaOfInterest(forMouse:) 

Instance Method

# areaOfInterest(forMouse:)

Returns the type of area the mouse cursor is over.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func areaOfInterest(forMouse event: UIEvent) -> PDFAreaOfInterest
```

**macOS**

``` source
@MainActor
func areaOfInterest(forMouse event: NSEvent) -> PDFAreaOfInterest
```

## Discussion

The `PDFAreaOfInterest` enumeration defines the various area types. This method is for custom subclasses of the `PDFView` class. Use it if you override the `NSResponder` class’s mouseMoved(with:) method or related methods.

Refer to `Constants` for the various values of the area-of-interest constants. Each of these constants contributes to the value of the `PDFAreaOfInterest` bit field.

## See Also

### Working with Mouse Position and Events

func areaOfInterest(for: CGPoint) -> PDFAreaOfInterest

Returns the type of area for a specific cursor location point.

struct PDFAreaOfInterest

The mouse position over PDF view areas.

func setCursorFor(PDFAreaOfInterest)

Sets the type of mouse cursor according to the type of area the mouse cursor is over.

func perform(PDFAction)

Performs the specified action.

Drag Operations

Define drag operations allowed for a view.

