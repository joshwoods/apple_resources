

- AppKit
-  NSWritingToolsResultOptions 

Structure

# NSWritingToolsResultOptions

Constants to specify what type of content to allow in Writing Tools suggestions or rewrites.

macOS 15.0+

``` source
struct NSWritingToolsResultOptions
```

## Overview

When configuring a text view, specify what type of text input you want Writing Tools to deliver to your view. You can ask it to return plain text without any attributes, or you can ask it to apply relevant formatting attributes to the text. You can even encourage it to return items in a list or format them in a table.

## Topics

### Getting the output options

static var plainText: NSWritingToolsResultOptions

An option to allow only plain text without any attributes in the returned text.

static var richText: NSWritingToolsResultOptions

An option to include style attributes consistent with the RTF format in the returned text.

static var list: NSWritingToolsResultOptions

An option to allow list-style formatting in the returned text.

static var table: NSWritingToolsResultOptions

An option to allow tabular layout attributes in the returned text.

### Initializers

init(rawValue: UInt)

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

### Enumerations

enum FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

enum NSHorizontalDirection

An absolute direction on the horizontal axis.

enum NSSharingCollaborationMode

Represents the types of sharing (collaborating on an item vs. sending a copy of the item) The share picker supports up to two modes, each of which corresponds to one of these types

enum DynamicRange

Describes how High Dynamic Range (HDR) image content displays.

enum NSTextCursorAccessoryPlacement

enum NSVerticalDirection

A direction on the vertical axis.

enum NSWritingToolsBehavior

Constants that specify the Writing Tools experience for the underlying view.

