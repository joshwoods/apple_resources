

- MapKit
-  MKUserLocationView 

Class

# MKUserLocationView

A configurable annotation that shows the user’s location using the default MapKit style.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
class MKUserLocationView
```

## Overview

If you don’t need additional configuration, you can show an annotation with the user’s location by setting showsUserLocation on the map to `true`.

If you want to specify additional configuration, such as zPriority, create this annotation view directly. To display the annotation view, return the instance from mapView(_:viewFor:).

The user location view provides the MapKit default style and behavior. The visual display varies with the level of authorization the user grants your app.

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

### User location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

class MKUserLocation

An annotation that reflects the user’s location on the map.

