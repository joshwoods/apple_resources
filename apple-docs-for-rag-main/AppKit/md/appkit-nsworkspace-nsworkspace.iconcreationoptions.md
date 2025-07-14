

- AppKit
- NSWorkspace
-  NSWorkspace.IconCreationOptions 

Structure

# NSWorkspace.IconCreationOptions

Constants that describe options for creating icons.

macOS

``` source
struct IconCreationOptions
```

## Overview

Use these constants with the setIcon(_:forFile:options:) method. You can combine these using the C bitwise OR operator.

## Topics

### Creation Options

static var excludeQuickDrawElementsIconCreationOption: NSWorkspace.IconCreationOptions

An option to suppress generation of the QuickDraw format icon representations that are used in macOS 10.0 through macOS 10.4.

static var exclude10_4ElementsIconCreationOption: NSWorkspace.IconCreationOptions

An option to suppress generation of the new higher resolution icon representations that are supported in macOS 10.4.

### Initializers

init(rawValue: UInt)

Initializes an icon creation option using the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing Icons

func icon(forFile: String) -> NSImage

Returns an image containing the icon for the specified file.

func icon(forFiles: [String]) -> NSImage?

Returns an image containing the icon for the specified files.

func icon(for: UTType) -> NSImage

Returns an image containing the icon for the specified content type.

func setIcon(NSImage?, forFile: String, options: NSWorkspace.IconCreationOptions) -> Bool

Sets the icon for the file or directory at the specified path.

