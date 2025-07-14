

- Core Location
- CLGeocoder
-  isGeocoding 

Instance Property

# isGeocoding

A Boolean value indicating whether the receiver is in the middle of geocoding its value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isGeocoding: Bool { get }
```

## Discussion

This property contains the value true if the process is ongoing or false if the process is done or has not yet been initiated.

## See Also

### Managing geocoding requests

func cancelGeocode()

Cancels a pending geocoding request.

