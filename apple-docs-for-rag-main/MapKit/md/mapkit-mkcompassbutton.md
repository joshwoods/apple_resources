

- MapKit
-  MKCompassButton 

Class

# MKCompassButton

A specialized view that displays the compass heading for its associated map.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
class MKCompassButton
```

## Overview

Use this class when you want to incorporate a standard compass button into your own view hierarchy. A compass button reflects the current orientation of its associated map view. Tapping the compass button reorients the map so that due north is at the top of the map view.

## Topics

### Creating a compass button

convenience init(mapView: MKMapView?)

Creates a compass button and associates it with the specified map view.

### Getting the compass attributes

var mapView: MKMapView?

The map view that provides the heading information for the compass button.

var compassVisibility: MKFeatureVisibility

The visibility of the compass button.

enum MKFeatureVisibility

Constants that indicate the visibility of different map features.

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

class MKScaleView

A specialized view that displays the scale information for its associated map.

class MKZoomControl

A specialized view that displays and controls the zoom level of the map view.

class MKPitchControl

A specialized view that displays and controls the pitch angle of the map view.

class MKUserTrackingButton

A specialized button that allows the user to toggle whether the map tracks to the heading the user is facing.

class MKUserTrackingBarButtonItem

A specialized bar button item that allows the user to toggle whether the map tracks to the heading the user is facing.

