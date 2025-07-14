

- MapKit
-  MKOverlayPathView Deprecated

Class

# MKOverlayPathView

Represents a generic overlay that draws its contents using a Core Graphics path data type.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class MKOverlayPathView
```

## Overview

You can use this class to implement simple path-based overlay views or subclass it to define additional drawing behaviors. The default drawing behavior of this class is to apply the object’s current fill attributes, fill the path, apply the current stroke attributes, and then stroke the path.

If you subclass, you should override the createPath method and use that method to build the appropriate path for the overlay. You can invalidate this path as needed and force the path to be recreated using whatever new data your subclass has obtained.

In iOS 7 and later, use the MKOverlayPathRenderer class to display path-based overlays instead.

## Relationships

### Inherits From

- MKOverlayView

### Inherited By

- MKCircleView
- MKPolygonView
- MKPolylineView

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

