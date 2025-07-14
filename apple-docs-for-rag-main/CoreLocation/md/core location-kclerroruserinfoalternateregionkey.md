

- Core Location
-  kCLErrorUserInfoAlternateRegionKey 

Global Variable

# kCLErrorUserInfoAlternateRegionKey

A key in the user information dictionary of an error relating to a delayed region-monitoring response.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
let kCLErrorUserInfoAlternateRegionKey: String
```

## Discussion

This key is included in an error of type regionMonitoringResponseDelayed. The value is a CLRegion object containing the region that location services can monitor more effectively.

## See Also

### Errors

struct CLError

A Core Location error.

let kCLErrorDomain: String

The domain for Core Location errors.

