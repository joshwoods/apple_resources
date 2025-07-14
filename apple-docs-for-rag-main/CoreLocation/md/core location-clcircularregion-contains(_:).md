

- Core Location
- CLCircularRegion
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the geographic area contains the specified coordinate.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.10–11.0DeprecatedtvOS 9.0+watchOS 2.0–9.0Deprecated

``` source
func contains(_ coordinate: CLLocationCoordinate2D) -> Bool
```

## Parameters 

`coordinate`  

The coordinate to test against the region.

## Return Value

Returns true if the coordinate lies within the region’s boundaries, or false if it doesn’t.

