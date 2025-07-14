

- MapKit
- MKPointOfInterestFilter
-  includes(\_:) 

Instance Method

# includes(\_:)

Returns a Boolean value indicating whether the filter includes the point of interest category.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func includes(_ category: MKPointOfInterestCategory) -> Bool
```

## Parameters 

`category`  

A point of interest category that the method checks for inclusion in the filter.

## Return Value

`true` if the filter includes the point of interest category; otherwise, `false`.

## See Also

### Querying filter behavior

func excludes(MKPointOfInterestCategory) -> Bool

Returns a Boolean value indicating whether the filter excludes the point of interest category.

