

- MapKit
- MKDirections
- MKDirections.Request
-  init(contentsOfURL:) 

Initializer

# init(contentsOfURL:)

Creates and returns a directions request object using the specified URL.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+

``` source
init(contentsOfURL url: URL)
```

``` source
init(contentsOf url: URL)
```

## Parameters 

`url`  

The URL provided to your app.

## Return Value

An initialized directions request object.

## Discussion

You should use the isDirectionsRequest(_:) method to verify that the specified URL is of the correct format before calling this method to initialize the object.

## See Also

### Creating a directions request object

class func isDirectionsRequest(URL) -> Bool

Returns a Boolean value that indicates whether the specified URL contains a directions request.

