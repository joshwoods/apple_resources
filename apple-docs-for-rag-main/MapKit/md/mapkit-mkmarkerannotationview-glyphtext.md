

- MapKit
- MKMarkerAnnotationView
-  glyphText 

Instance Property

# glyphText

The text to display in the marker balloon.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var glyphText: String? { get set }
```

## Discussion

Use this property or the glyphText property to specify the marker balloon content. If you specify both an image and text, MapKit displays the text.

MapKit limits the amount of space available for displaying your glyph text. Specify no more than two or three characters for any strings you assign to this property.

## See Also

### Setting the Marker Content

var glyphImage: UIImage?

An image to display in the marker balloon.

var glyphTintColor: UIColor?

The color to apply to the glyph text or image.

var selectedGlyphImage: UIImage?

An image to display when the user selects the marker.

