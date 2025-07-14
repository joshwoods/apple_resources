

- MapKit
- MKPointOfInterestFilter
-  init(including:) 

Initializer

# init(including:)

Initialize the point of interest filter with a list of categories to include.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
init(including categories: [MKPointOfInterestCategory])
```

## Parameters 

`categories`  

An array of categories to include.

## See Also

### Creating filters

class var excludingAll: MKPointOfInterestFilter

A filter that excludes all point of interest categories.

class var includingAll: MKPointOfInterestFilter

A filter that includes all point of interest categories.

init(excluding: [MKPointOfInterestCategory])

Initialize the point of interest filter with a list of categories to exclude.

