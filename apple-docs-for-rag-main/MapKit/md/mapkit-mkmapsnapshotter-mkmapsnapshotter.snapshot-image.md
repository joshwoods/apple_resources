

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Snapshot
-  image 

Instance Property

# image

The image of the map’s content.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**macOS**

``` source
var image: NSImage { get }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var image: UIImage { get }
```

## Discussion

The image object contains representations appropriate for display on both Retina and standard displays.

## See Also

### Getting the snapshot image

var appearance: NSAppearance

The visual style that MapKit uses when rendering the snapshot.

