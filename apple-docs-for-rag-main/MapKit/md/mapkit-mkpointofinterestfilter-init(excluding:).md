

- MapKit
- MKPointOfInterestFilter
-  init(excluding:) 

Initializer

# init(excluding:)

Initialize the point of interest filter with a list of categories to exclude.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
init(excluding categories: [MKPointOfInterestCategory])
```

## Parameters 

`categories`  

An array of categories to exclude.

## See Also

### Creating filters

class var excludingAll: MKPointOfInterestFilter

A filter that excludes all point of interest categories.

class var includingAll: MKPointOfInterestFilter

A filter that includes all point of interest categories.

init(including: [MKPointOfInterestCategory])

Initialize the point of interest filter with a list of categories to include.

