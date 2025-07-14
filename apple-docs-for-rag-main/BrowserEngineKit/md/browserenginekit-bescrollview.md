

- BrowserEngineKit
-  BEScrollView 

Class

# BEScrollView

A scroll view that works with its delegate to handle nesting, and customize scroll interactions.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
class BEScrollView
```

## Overview

Use `BEScrollView` instead of UIScrollView in situations where you need to:

- Handle scroll updates programmatically, potentially overriding the default scroll view behavior.

- Have scroll views that are siblings in the view hierarchy but nested in the browser Document Object Model (DOM).

If either of these is true, replace your use of `UIScrollView` with `BEScrollView` and set the scroll view’s delegate to an object that implements the BEScrollViewDelegate methods.

## Topics

### Responding to scroll updates

var delegate: (any BEScrollViewDelegate)?

The delegate of the scroll view.

## Relationships

### Inherits From

- UIScrollView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIFocusItemScrollableContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Scroll view interaction

class BEScrollViewScrollUpdate

An object that represents a change in a scroll view’s scroll state.

protocol BEScrollViewDelegate

The protocol that browser scroll view delegates conform to.

