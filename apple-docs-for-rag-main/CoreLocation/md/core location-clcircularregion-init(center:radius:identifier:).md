

- Core Location
- CLCircularRegion
-  init(center:radius:identifier:) 

Initializer

# init(center:radius:identifier:)

Creates and returns a region object defining a circular geographic area.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.10–11.0DeprecatedtvOS 9.0+watchOS 2.0–9.0Deprecated

``` source
init(
    center: CLLocationCoordinate2D,
    radius: CLLocationDistance,
    identifier: String
)
```

## Parameters 

`center`  

The center point of the geographic region to monitor.

`radius`  

The distance (measured in meters) from the center point of the geographic region to the edge of the circular boundary.

`identifier`  

A unique identifier to associate with the region object. You use this identifier to differentiate regions within your app. This value can’t be `nil`.

## Return Value

An initialized region object.

## Discussion

When defining a geographic region, remember that the location manager doesn’t generate notifications immediately upon crossing a region boundary. Instead, it applies time and distance criteria to ensure that the crossing is intentional and needs to trigger a notification. So choose a center point and radius that are appropriate and give you enough time to alert the user. For more information, see the information about region monitoring in Location and Maps Programming Guide.

