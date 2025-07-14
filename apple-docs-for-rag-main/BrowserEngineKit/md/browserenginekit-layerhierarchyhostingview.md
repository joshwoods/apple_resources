

- BrowserEngineKit
-  LayerHierarchyHostingView 

Class

# LayerHierarchyHostingView

A view that hosts a layer hierarchy you manage in another process.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
class LayerHierarchyHostingView
```

## Mentioned in 

Propagating view visibility information to extension processes

Hosting browser view layers in the rendering extension

## Overview

Set the view’s handle to a LayerHierarchyHandle you get from the other process. When you invalidate the associated layer hierarchy, you need to stop displaying the view.

## Topics

### Identifying remote layer hierarchy

var handle: LayerHierarchyHandle?

A handle that refers to a layer hierarchy in another process.

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

### Layer hosting

Hosting browser view layers in the rendering extension

Coordinate view-hierarchy and layer-hierarchy changes between processes.

class LayerHierarchy

An object that holds a reference to layers rendered in another process’s view.

class LayerHierarchyHostingTransactionCoordinator

Synchronizes updates to views and layers in different processes.

class LayerHierarchyHandle

A reference to a layer hierarchy that you share between processes.

