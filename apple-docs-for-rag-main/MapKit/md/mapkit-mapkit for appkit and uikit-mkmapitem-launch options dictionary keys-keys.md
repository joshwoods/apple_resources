

- MapKit
- MapKit for AppKit and UIKit
- MKMapItem
-  Launch options dictionary keys 

API Collection

# Launch options dictionary keys

Launch options to specify when opening map items in the Maps app.

## Overview

You specify these keys in the launch options dictionary for the openMaps(with:launchOptions:) or openInMaps(launchOptions:) method.

## Topics

### Launch options

let MKLaunchOptionsDirectionsModeKey: String

The mode of transportation.

let MKLaunchOptionsMapTypeKey: String

The type of map (standard, satellite, or hybrid) to display.

let MKLaunchOptionsMapCenterKey: String

The coordinate value on which to center the map.

let MKLaunchOptionsMapSpanKey: String

The amount of the map to display.

let MKLaunchOptionsShowsTrafficKey: String

A Boolean value that indicates whether to display traffic information.

let MKLaunchOptionsCameraKey: String

The virtual camera to use for viewing the map.

## See Also

### Opening items at launch time

Directions mode values

Strings that represent the possible values of the launch options direction mode key.

