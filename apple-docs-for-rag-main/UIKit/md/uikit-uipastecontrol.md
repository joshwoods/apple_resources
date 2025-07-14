

- UIKit
-  UIPasteControl 

Class

# UIPasteControl

A button that a person taps to place pasteboard contents in your app.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class UIPasteControl
```

## Overview

You can configure the button to appear as an icon, text, or both. The following button represents the icon and text option:

In iOS 16 and later, programmatic pasting raises a user alert that prompts the user for approval before the app gains access to pasteboard contents (`UIPasteboard.general.string`). Use this class to paste without a user prompt.

### Add a paste button to a text view

The following code displays a paste button and assigns a text view as the recipient of pasteboard contents:

```
let textView = UITextView(frame: view.bounds)
view.addSubview(textView)

let configuration = UIPasteControl.Configuration()
configuration.baseBackgroundColor = .red
configuration.baseForegroundColor = .magenta
configuration.cornerStyle = .capsule
configuration.displayMode = .iconAndLabel

let pasteButton = UIPasteControl(configuration: configuration)
pasteButton.frame = CGRect(x: view.bounds.width/2.0, y: view.bounds.height/2.0, width: 150, height: 60)
textView.addSubview(pasteButton)

pasteButton.target = textView
```

## Topics

### Creating a paste button

init?(coder: NSCoder)

Creates a paste button by deserializing the specified coder.

init(configuration: UIPasteControl.Configuration)

Creates a paste button that conforms to the specified configuration.

init(frame: CGRect)

Creates a paste button with the specified size and position.

### Identifying the content recipient

var target: (any UIPasteConfigurationSupporting)?

The UI control that receives pasted content.

### Determining the button’s look

var configuration: UIPasteControl.Configuration

An object that customizes the look of the paste button.

class Configuration

An object that determines a paste button’s color, corner style, icon, and text.

## Relationships

### Inherits From

- UIControl

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
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Pasteboard

class Configuration

An object that determines a paste button’s color, corner style, icon, and text.

enum DisplayMode

Options that determine whether a paste button composes an icon, textual label, or both.

class UIPasteboard

An object that helps a user share data from one place to another within your app, and from your app to other apps.

class UIPasteConfiguration

The interface that an object implements to declare its ability to accept specific data types for pasting and for drag-and-drop activities.

protocol UIPasteConfigurationSupporting

The interface that determines whether a responder object supports paste configuration.

