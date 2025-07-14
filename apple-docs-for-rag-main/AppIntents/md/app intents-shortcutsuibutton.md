

- App Intents
-  ShortcutsUIButton 

Class

# ShortcutsUIButton

A button that opens the current app’s page in the Shortcuts app.

AppIntentsUIKitiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor @objc @preconcurrency
final class ShortcutsUIButton
```

## Overview

You can add additional targets to observe when the button is tapped.

## Topics

### Creating the button

init(style: ShortcutsLinkStyle)

Creates a button with the specified style.

### Getting the button style

var style: ShortcutsLinkStyle

The style to use for the button.

### Configuring additional actions

func addTarget(Any?, action: Selector, for: UIControl.Event)

### Resizing the button

func sizeThatFits(CGSize) -> CGSize

## Relationships

### Inherits From

- UIButton

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
- UIAccessibilityContentSizeCategoryImageAdjusting
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UIContextMenuInteractionDelegate
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UISpringLoadedInteractionSupporting
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Buttons

struct ShortcutsLink

A button that brings users to the current app’s App Shortcuts page in the Shortcuts app.

struct ShortcutsLinkStyle

The styles to apply to buttons you use to open your app’s page in the Shortcuts app.

