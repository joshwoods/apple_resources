

- MapKit
-  MKOverlayView Deprecated

Class

# MKOverlayView

Defines the basic behavior associated with all overlay views.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class MKOverlayView
```

## Overview

An overlay view provides the visual representation of an overlay object—that is, an object that conforms to the MKOverlay protocol. This class defines the drawing infrastructure used by the map view but does not do any actual drawing. Subclasses are expected to override the drawMapRect:zoomScale:inContext: method in order to draw the contents of the overlay view.

The Map Kit framework provides several concrete instances of overlay views. Specifically, it provides overlay views for each of the concrete overlay objects. You can use one of these existing overlay views or define your own subclass if you want to draw the overlay contents differently.

In iOS 7 and later, use the MKOverlayRenderer class to display overlays instead.

### Subclassing notes

You can subclass `MKOverlayView` to create overlays based on custom shapes and content. The only method subclasses are expected to override is the drawMapRect:zoomScale:inContext: method. However, if your class contains content that may not be ready for drawing right away, you should also override the canDrawMapRect:zoomScale: method and use it to report when your class is ready and able to draw.

The implementation of your drawMapRect:zoomScale:inContext: method must be safe to run from multiple threads simultaneously. To improve performance, the map view may tile overlays that are large enough and distribute the rendering of each tile to separate threads.

## Relationships

### Inherits From

- UIView

### Inherited By

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

