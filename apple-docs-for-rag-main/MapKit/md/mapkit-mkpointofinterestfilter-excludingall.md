

- MapKit
- MKPointOfInterestFilter
-  excludingAll 

Type Property

# excludingAll

A filter that excludes all point of interest categories.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class var excludingAll: MKPointOfInterestFilter { get }
```

## Discussion

You can use excludingAll to remove all points of interest from your map view without listing all the categories individually.

## See Also

### Creating filters

class var includingAll: MKPointOfInterestFilter

A filter that includes all point of interest categories.

init(excluding: [MKPointOfInterestCategory])

Initialize the point of interest filter with a list of categories to exclude.

init(including: [MKPointOfInterestCategory])

Initialize the point of interest filter with a list of categories to include.

