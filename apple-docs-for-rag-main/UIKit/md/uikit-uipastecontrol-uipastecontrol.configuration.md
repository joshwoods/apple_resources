

- UIKit
- UIPasteControl
-  UIPasteControl.Configuration 

Class

# UIPasteControl.Configuration

An object that determines a paste button’s color, corner style, icon, and text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class Configuration
```

## Overview

The paste button (UIPasteControl) property configuration is of this type.

## Topics

### Coloring the button

var baseBackgroundColor: UIColor?

A color for the paste button’s background.

var baseForegroundColor: UIColor?

A color for the paste button’s icon and text.

### Shaping button corners

var cornerRadius: CGFloat

A value that rounds the edges of a paste button.

var cornerStyle: UIButton.Configuration.CornerStyle

A shape for the button among a predetermined set of templates.

### Choosing control icon and text

var displayMode: UIPasteControl.DisplayMode

An option that determines whether the paste button composes an icon, textual label, or both.

enum DisplayMode

Options that determine whether a paste button composes an icon, textual label, or both.

### Instance Properties

var imagePlacement: NSDirectionalRectEdge

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Pasteboard

class UIPasteControl

A button that a person taps to place pasteboard contents in your app.

enum DisplayMode

Options that determine whether a paste button composes an icon, textual label, or both.

class UIPasteboard

An object that helps a user share data from one place to another within your app, and from your app to other apps.

class UIPasteConfiguration

The interface that an object implements to declare its ability to accept specific data types for pasting and for drag-and-drop activities.

protocol UIPasteConfigurationSupporting

The interface that determines whether a responder object supports paste configuration.

