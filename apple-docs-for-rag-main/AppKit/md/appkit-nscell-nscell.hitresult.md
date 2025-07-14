

- AppKit
- NSCell
-  NSCell.HitResult 

Structure

# NSCell.HitResult

Constants used by the hitTest(for:in:of:) method to determine the effect of an event.

macOS 10.5+

``` source
struct HitResult
```

## Topics

### Constants

static var contentArea: NSCell.HitResult

A content area in the cell.

static var editableTextArea: NSCell.HitResult

An editable text area of the cell.

static var trackableArea: NSCell.HitResult

A trackable area in the cell.

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

struct StyleMask

Constants for specifying what happens when a button is pressed or is displaying its alternate state.

enum NSControlTint

Constants for specifying a cell’s tint color.

enum ControlSize

A constant for specifying a cell’s size.

enum BackgroundStyle

Background styles to apply to a view’s cell.

Deprecated Scaling Constants

These are deprecated scaling constants.

Data Entry Types

These constants specify how a cell formats numeric data.

