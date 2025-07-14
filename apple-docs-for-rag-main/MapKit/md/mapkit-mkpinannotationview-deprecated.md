

- MapKit
-  MKPinAnnotationView Deprecated

Class

# MKPinAnnotationView

An annotation view that displays a pin image on the map.

iOS 3.0–16.0DeprecatediPadOS 3.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.9–13.0DeprecatedtvOS 9.2–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class MKPinAnnotationView
```

Deprecated

In iOS 16 and macOS 13 and later use an MKAnnotationView to create a custom map annotation

## Overview

Return instances of this class from the mapView(_:viewFor:) method of your map view delegate when you want to display a pin for one of your annotations. The pins displayed by this view are the same ones found in the Maps application. You can specify the type of pin you want to display and whether you want the pin to be animated into place.

Note

In iOS 5.1 and earlier, the MapKit framework uses the Google Mobile Maps (GMM) service to provide map data. Use of specific classes of this framework (and their associated interfaces) is subject to the Google Mobile Maps terms of service, found at http://code.google.com/apis/maps/iphone/terms.html.

## Topics

### Getting Standard Pin Colors

class func redPinColor() -> UIColor

Returns the standard color for red pins.

class func greenPinColor() -> UIColor

Returns the standard color for green pins.

class func purplePinColor() -> UIColor

Returns the standard color for purple pins.

enum MKPinAnnotationColor

The supported colors for pin annotations.

### Getting and Setting Attributes

var pinTintColor: UIColor!

The color of the pin head.

var animatesDrop: Bool

A Boolean value indicating whether the annotation view is animated onto the screen.

var pinColor: MKPinAnnotationColor

The color of the pin head.

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

class MKMarkerAnnotationView

An annotation view that displays a balloon-shaped marker at the designated location.

