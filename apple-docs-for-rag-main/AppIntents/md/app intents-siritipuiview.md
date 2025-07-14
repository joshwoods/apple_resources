

- App Intents
-  SiriTipUIView 

Class

# SiriTipUIView

A view that displays the phrase a person uses to invoke an App Shortcut.

AppIntentsUIKitiOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor @objc @preconcurrency
final class SiriTipUIView
```

## Overview

You must call `UISiriTip/setIntent(intent:)` before displaying the view.

## Topics

### Creating a tip view

init(style: SiriTipViewStyle)

A view that displays the phrase for an App Shortcut.

### Getting the view style

var style: SiriTipViewStyle

The style to use for the view.

struct SiriTipViewStyle

The styles to apply to the tip views you use to display spoken phrases.

### Getting the view’s configuration

var allowsDismissal: Bool

Indicates if the tip view should display a dismissal button

var isPresented: Bool

Determines if the view should be presented to the user.

### Instance Properties

var intrinsicContentSize: CGSize

### Instance Methods

func didMoveToWindow()

func setIntent&lt;Intent>(intent: Intent)

Sets an `AppIntent` for this view. This must be called before presenting the view.

func sizeThatFits(CGSize) -> CGSize

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

### Tip views

struct SiriTipView

A SwiftUI view that displays the phrase someone uses to invoke an App Shortcut.

struct SiriTipViewStyle

The styles to apply to the tip views you use to display spoken phrases.

