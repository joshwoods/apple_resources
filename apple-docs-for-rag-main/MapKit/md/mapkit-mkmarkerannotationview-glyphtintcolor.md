

- MapKit
- MKMarkerAnnotationView
-  glyphTintColor 

Instance Property

# glyphTintColor

The color to apply to the glyph text or image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
@NSCopying @MainActor
var glyphTintColor: NSColor? { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@NSCopying @MainActor
var glyphTintColor: UIColor? { get set }
```

## Discussion

The default value of this property is `nil`, which applies the standard tint color for the current map style.

## See Also

### Setting the Marker Content

var glyphText: String?

The text to display in the marker balloon.

var glyphImage: UIImage?

An image to display in the marker balloon.

var selectedGlyphImage: UIImage?

An image to display when the user selects the marker.

