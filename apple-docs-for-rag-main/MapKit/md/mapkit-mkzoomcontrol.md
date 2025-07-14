

- MapKit
-  MKZoomControl 

Class

# MKZoomControl

A specialized view that displays and controls the zoom level of the map view.

Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor
class MKZoomControl
```

## Overview

Use this class when you want to incorporate a standard, fixed-size zoom control into your own view hierarchy. A zoom control enables the user to change the zoom level of its associated map view.

## Topics

### Creating a zoom control

convenience init(mapView: MKMapView?)

Creates a zoom control and associates it with the specified map view.

### Accessing the map view

var mapView: MKMapView?

The map view associated with this control.

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
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

class MKPitchControl

A specialized view that displays and controls the pitch angle of the map view.

class MKUserTrackingButton

A specialized button that allows the user to toggle whether the map tracks to the heading the user is facing.

class MKUserTrackingBarButtonItem

A specialized bar button item that allows the user to toggle whether the map tracks to the heading the user is facing.

