

- MapKit
-  MKMarkerAnnotationView 

Class

# MKMarkerAnnotationView

An annotation view that displays a balloon-shaped marker at the designated location.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class MKMarkerAnnotationView
```

## Overview

Return an instance of this class from the mapView(_:viewFor:) method of your map view delegate when you want to display the same types of markers used in the Maps app.

The default displayPriority for an instance of this class is defaultLow.

## Topics

### Setting the Marker Color

var markerTintColor: UIColor?

The background color of the marker balloon.

### Setting the Marker Content

var glyphText: String?

The text to display in the marker balloon.

var glyphImage: UIImage?

An image to display in the marker balloon.

var glyphTintColor: UIColor?

The color to apply to the glyph text or image.

var selectedGlyphImage: UIImage?

An image to display when the user selects the marker.

### Setting the Visibility

var titleVisibility: MKFeatureVisibility

The visibility of the title text rendered beneath the marker balloon.

var subtitleVisibility: MKFeatureVisibility

The visibility of the subtitle text rendered beneath the marker balloon.

enum MKFeatureVisibility

Constants that indicate the visibility of different map features.

### Animating the Marker onto the Screen

var animatesWhenAdded: Bool

A Boolean that indicates whether the marker animates into position onscreen.

## Relationships

### Inherits From

- MKAnnotationView

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

### Location annotations

Annotating a Map with Custom Data

Annotate a map with location-specific data using default and customized annotation views and callouts.

class MKPointAnnotation

A string-based piece of location-specific data that you apply to a specific point on a map.

class MKMapItemAnnotation

An annotation that represents a map item

class MKPinAnnotationView

An annotation view that displays a pin image on the map.

Deprecated

