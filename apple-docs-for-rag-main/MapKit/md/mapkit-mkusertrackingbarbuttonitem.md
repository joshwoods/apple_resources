

- MapKit
-  MKUserTrackingBarButtonItem 

Class

# MKUserTrackingBarButtonItem

A specialized bar button item that allows the user to toggle whether the map tracks to the heading the user is facing.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class MKUserTrackingBarButtonItem
```

## Overview

Tapping the button lets the user toggles between modes for displaying the map with and without the current heading applied. The button also reflects the current user tracking mode if set elsewhere. This bar button item is associated to a single map view.

## Topics

### Creating a user tracking bar button item

init(mapView: MKMapView?)

Initializes a newly created bar button item with the specified map view.

### Accessing the owning map

var mapView: MKMapView?

The map view associated with this bar button item.

## Relationships

### Inherits From

- UIBarButtonItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- UIAccessibilityIdentification
- UIAppearance
- UIPopoverPresentationControllerSourceItem
- UISpringLoadedInteractionSupporting

## See Also

### Map customization

class MKMapCamera

A virtual camera for defining the appearance of the map.

class MKCompassButton

A specialized view that displays the compass heading for its associated map.

class MKScaleView

A specialized view that displays the scale information for its associated map.

class MKZoomControl

A specialized view that displays and controls the zoom level of the map view.

class MKPitchControl

A specialized view that displays and controls the pitch angle of the map view.

class MKUserTrackingButton

A specialized button that allows the user to toggle whether the map tracks to the heading the user is facing.

