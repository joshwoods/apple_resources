

- MapKit
- MKDirections
- MKDirections.Request
-  isDirectionsRequest(\_:) 

Type Method

# isDirectionsRequest(\_:)

Returns a Boolean value that indicates whether the specified URL contains a directions request.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+

``` source
class func isDirectionsRequest(_ url: URL) -> Bool
```

## Parameters 

`url`  

The URL the system provides to your app.

## Return Value

true if the URL contains a directions request that your app needs to display to the user, or false if it doesn’t.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating a directions request object

init(contentsOfURL: URL)

Creates and returns a directions request object using the specified URL.

