

- CoreAudioKit
-  AUGenericViewInternal 

Class

# AUGenericViewInternal

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 13.0+visionOS

``` source
@MainActor @objc @preconcurrency
class AUGenericViewInternal
```

## Overview

Apple discourages the use of this symbol.

## Topics

### Initializers

init?(coder: NSCoder)

init(frame: CGRect)

### Instance Properties

var auAudioUnit: AUAudioUnit?

var owningController: UIViewController?

var paramObserverToken: AUParameterObserverToken?

var showSingleClumpIndex: Int?

### Instance Methods

func removeFromSuperview()

func removeScheduledUpdatesTimer()

func traitCollectionDidChange(UITraitCollection?)

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSCollectionViewDelegate
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
- UICollectionViewDelegate
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UIScrollViewDelegate
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Deprecations

typealias AUGenericViewInternalBase

