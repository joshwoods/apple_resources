

- AppKit
- NSCell
-  NSCell.StyleMask 

Structure

# NSCell.StyleMask

Constants for specifying what happens when a button is pressed or is displaying its alternate state.

macOS

``` source
struct StyleMask
```

## Overview

These contents are used by the highlightsBy and showsStateBy methods of NSButtonCell.

## Topics

### Constants

static var pushInCellMask: NSCell.StyleMask

The button cell “pushes in” if it has a border.

static var contentsCellMask: NSCell.StyleMask

The button cell displays its alternate icon and/or title.

static var changeGrayCellMask: NSCell.StyleMask

The button cell swaps the “control color” (the controlColor method of `NSColor`) and white pixels on its background and icon.

static var changeBackgroundCellMask: NSCell.StyleMask

Same as `NSChangeGrayCellMask`, but only background pixels are changed.

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

### Constants

enum CellType

Constants for specifying how a cell represents its data (as text or as an image).

enum Attribute

Constants for specifying how a button behaves when pressed and how it displays its state.

enum ImagePosition

A constant for specifying the position of a button’s image relative to its title.

enum NSImageScaling

Constants that specify a cell’s image scaling behavior.

typealias StateValue

Constants for specifying a cell’s state and are used mostly for buttons.

Deprecated

enum NSControlTint

Constants for specifying a cell’s tint color.

enum ControlSize

A constant for specifying a cell’s size.

struct HitResult

Constants used by the hitTest(for:in:of:) method to determine the effect of an event.

enum BackgroundStyle

Background styles to apply to a view’s cell.

Deprecated Scaling Constants

These are deprecated scaling constants.

Data Entry Types

These constants specify how a cell formats numeric data.

