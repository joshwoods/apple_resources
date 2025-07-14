

- MapKit
- MKDistanceFormatter
-  string(fromDistance:) 

Instance Method

# string(fromDistance:)

Creates a string representation of the specified distance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
func string(fromDistance distance: CLLocationDistance) -> String
```

## Parameters 

`distance`  

The distance value that you want to convert to a string.

## Return Value

A user-readable string that describes the distance based on the formatter settings.

## See Also

### Converting distances

func distance(from: String) -> CLLocationDistance

Returns the distance value parsed from the specified string.

