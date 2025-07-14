

- UIKit
- UIPasteControl
-  UIPasteControl.DisplayMode 

Enumeration

# UIPasteControl.DisplayMode

Options that determine whether a paste button composes an icon, textual label, or both.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum DisplayMode
```

## Overview

The paste button (UIPasteControl) property displayMode is of this type.

## Topics

### Choosing a display mode

case iconAndLabel

A display mode for a button that composes an icon and a textual label.

case iconOnly

A display mode for an icon button.

case labelOnly

A display mode for a textual label.

### Enumeration Cases

case arrowAndLabel

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Pasteboard

class UIPasteControl

A button that a person taps to place pasteboard contents in your app.

class Configuration

An object that determines a paste button’s color, corner style, icon, and text.

class UIPasteboard

An object that helps a user share data from one place to another within your app, and from your app to other apps.

class UIPasteConfiguration

The interface that an object implements to declare its ability to accept specific data types for pasting and for drag-and-drop activities.

protocol UIPasteConfigurationSupporting

The interface that determines whether a responder object supports paste configuration.

