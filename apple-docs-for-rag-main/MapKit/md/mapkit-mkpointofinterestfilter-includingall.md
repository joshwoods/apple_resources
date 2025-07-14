

- MapKit
- MKPointOfInterestFilter
-  includingAll 

Type Property

# includingAll

A filter that includes all point of interest categories.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class var includingAll: MKPointOfInterestFilter { get }
```

## Discussion

You can use includingAll to include all points of interest in your map view without listing all the categories individually.

## See Also

### Creating filters

class var excludingAll: MKPointOfInterestFilter

A filter that excludes all point of interest categories.

init(excluding: [MKPointOfInterestCategory])

Initialize the point of interest filter with a list of categories to exclude.

init(including: [MKPointOfInterestCategory])

Initialize the point of interest filter with a list of categories to include.

