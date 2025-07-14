

- AppKit
- NSTextField
-  NSTextField.BezelStyle 

Enumeration

# NSTextField.BezelStyle

The style of bezel the text field displays.

macOS

``` source
enum BezelStyle
```

## Overview

Use bezelStyle to set a text field’s bezel style.

## Topics

### Constants

case squareBezel

A style that draws a bezel with square corners around a text field.

case roundedBezel

A style that draws a bezel with rounded corners around a single-line text field.

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

### Controlling the Background

var backgroundColor: NSColor?

The color of the background the text field’s cell draws behind the text.

var drawsBackground: Bool

A Boolean value that controls whether the text field’s cell draws a background color behind the text.

var isBezeled: Bool

A Boolean value that controls whether the text field draws a bezeled background around its contents.

var bezelStyle: NSTextField.BezelStyle

The text field’s bezel style, square or rounded.

