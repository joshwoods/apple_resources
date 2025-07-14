

- MapKit
-  MKPolylineView Deprecated

Class

# MKPolylineView

Provides the visual representation for an MKPolyline annotation object.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class MKPolylineView
```

## Overview

This view strokes the path represented by the annotation. (This class does not fill the area enclosed by the path.) You can change the color and other drawing attributes of the path by modifying the properties inherited from the MKOverlayPathView class. This class is typically used as is and not subclassed.

In iOS 7 and later, use the MKPolylineRenderer class to display polyline overlays instead.

## Relationships

### Inherits From

- MKOverlayPathView

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

