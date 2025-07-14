

- MapKit
-  MKLaunchOptionsCameraKey 

Global Variable

# MKLaunchOptionsCameraKey

The virtual camera to use for viewing the map.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 2.0+

``` source
let MKLaunchOptionsCameraKey: String
```

## Discussion

The value of this key is an MKMapCamera object that describes a virtual camera that can specify a 3D perspective for the map. If you don’t specify this key, the Maps app uses its current settings to define the appearance of the map.

## See Also

### Launch options

let MKLaunchOptionsDirectionsModeDefault: String

Directions that match the user’s preferred transportation type.

let MKLaunchOptionsDirectionsModeDriving: String

Driving directions between the specified start and end points.

let MKLaunchOptionsDirectionsModeKey: String

The mode of transportation.

let MKLaunchOptionsDirectionsModeTransit: String

Public transit directions between the specified start and end points.

let MKLaunchOptionsDirectionsModeWalking: String

Walking directions between the specified start and end points.

let MKLaunchOptionsMapCenterKey: String

The coordinate value on which to center the map.

let MKLaunchOptionsMapSpanKey: String

The amount of the map to display.

let MKLaunchOptionsMapTypeKey: String

The type of map (standard, satellite, or hybrid) to display.

let MKLaunchOptionsShowsTrafficKey: String

A Boolean value that indicates whether to display traffic information.

