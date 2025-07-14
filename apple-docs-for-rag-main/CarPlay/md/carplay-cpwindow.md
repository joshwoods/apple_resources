

- CarPlay
-  CPWindow 

Class

# CPWindow

A window that displays its content on the CarPlay screen.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
@MainActor
class CPWindow
```

## Overview

Navigation apps use a window to render their maps, and CarPlay provides one via the scene delegate’s templateApplicationScene(_:didConnect:to:) method. For all other categories of apps, you use templates exclusively to draw your user interface, and your scene delegate must implement templateApplicationScene(_:didConnect:) instead.

When CarPlay launches your navigation app, instantiate your map-drawing view controller and assign it to the window’s rootViewController property. This becomes the base CarPlay view and is for drawing maps exclusively. You use templates for all other user interface elements.

The base view of a navigation app does not receive tap or drag events.

## Topics

### Accessing the Scene

var templateApplicationScene: CPTemplateApplicationScene?

The application scene that contains the window.

### Layout

var mapButtonSafeAreaLayoutGuide: UILayoutGuide

The layout guide that represents the portion of the map template that map buttons don’t obscure.

## Relationships

### Inherits From

- UIWindow

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

### Accessing the Window

var carWindow: CPWindow

The window that belongs to the scene.

