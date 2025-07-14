

- AppKit
- NSCell
-  NSCell.Attribute 

Enumeration

# NSCell.Attribute

Constants for specifying how a button behaves when pressed and how it displays its state.

macOS

``` source
enum Attribute
```

## Overview

These constants are used by the NSButton and NSButtonCell classes.

## Topics

### Constants

case cellAllowsMixedState

Lets the cell’s state be `NSMixedState`, as well as `NSOffState` and `NSOnState`.

case changeBackgroundCell

If the cell’s state is `NSMixedState` or `NSOnState`, changes the cell’s background color from gray to white.

case cellChangesContents

If the cell’s state is `NSMixedState` or `NSOnState`, displays the cell’s alternate image.

case changeGrayCell

If the cell’s state is `NSMixedState` or `NSOnState`, displays the cell’s image as darkened.

case cellDisabled

Does not let the user manipulate the cell.

case cellEditable

Lets the user edit the cell’s contents.

case cellHasImageHorizontal

Controls the position of the cell’s image: places the image on the right of any text in the cell.

case cellHasImageOnLeftOrBottom

Controls the position of the cell’s image: places the image on the left of or below any text in the cell.

case cellHasOverlappingImage

Controls the position of the cell’s image: places the image over any text in the cell.

case cellHighlighted

Draws the cell with a highlighted appearance.

Deprecated

case cellIsBordered

Draws a border around the cell.

case cellIsInsetButton

Insets the cell’s contents from the border.

case cellLightsByBackground

If the cell is pushed in, changes the cell’s background color from gray to white.

case cellLightsByContents

If the cell is pushed in, displays the cell’s alternate image.

case cellLightsByGray

If the cell is pushed in, displays the cell’s image as darkened.

case pushInCell

Determines whether the cell’s image and text appear to be shifted down and to the right.

case cellState

The cell’s state.

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

### Constants

enum CellType

Constants for specifying how a cell represents its data (as text or as an image).

enum ImagePosition

A constant for specifying the position of a button’s image relative to its title.

enum NSImageScaling

Constants that specify a cell’s image scaling behavior.

typealias StateValue

Constants for specifying a cell’s state and are used mostly for buttons.

Deprecated

struct StyleMask

Constants for specifying what happens when a button is pressed or is displaying its alternate state.

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

