

- MapKit
-  MKScaleView 

Class

# MKScaleView

A specialized view that displays the scale information for its associated map.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class MKScaleView
```

## Overview

Use this class when you want to incorporate a standard scale view into your own view hierarchy. A scale view displays a legend with distance information for its associated map view. As the map region changes, the scale view updates automatically to reflect any changes in scale.

## Topics

### Creating a scale view

convenience init(mapView: MKMapView?)

Creates a scale view and associates it with the specified map view.

### Getting the scale view attributes

var mapView: MKMapView?

The map view that provides the scale information to the scale view.

var scaleVisibility: MKFeatureVisibility

The visibility of the scale view.

var legendAlignment: MKScaleView.Alignment

The alignment of the distance information in the scale view.

enum Alignment

Constants indicating whether measurements begin at the leading or trailing edge of the view.

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

class MKZoomControl

A specialized view that displays and controls the zoom level of the map view.

class MKPitchControl

A specialized view that displays and controls the pitch angle of the map view.

class MKUserTrackingButton

A specialized button that allows the user to toggle whether the map tracks to the heading the user is facing.

class MKUserTrackingBarButtonItem

A specialized bar button item that allows the user to toggle whether the map tracks to the heading the user is facing.

