

- MapKit
-  MKUserTrackingButton 

Class

# MKUserTrackingButton

A specialized button that allows the user to toggle whether the map tracks to the heading the user is facing.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class MKUserTrackingButton
```

## Overview

Use this class when you need a standard button that you can incorporate into your view hierarchy. Tapping the button lets the user toggles between modes for displaying the map with and without the current heading applied. The button also reflects the current user tracking mode if set elsewhere.

## Topics

### Creating a user tracking button

convenience init(mapView: MKMapView?)

Initializes the button with the map view that it should control.

### Getting the parent map

var mapView: MKMapView?

The map view associated with the button.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

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

class MKUserTrackingBarButtonItem

A specialized bar button item that allows the user to toggle whether the map tracks to the heading the user is facing.

