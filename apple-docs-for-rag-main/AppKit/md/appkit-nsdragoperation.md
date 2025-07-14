

- AppKit
-  NSDragOperation 

Structure

# NSDragOperation

A group of constants that represent which operations the dragging source can perform on dragging items.

macOS

``` source
struct NSDragOperation
```

## Topics

### Constants

static var copy: NSDragOperation

A constant that indicates the drag can copy the data that the image represents.

static var link: NSDragOperation

A constant that indicates the drag can share the data.

static var generic: NSDragOperation

A constant that indicates the destination can define the drag operation.

static var `private`: NSDragOperation

A constant that indicates the source and destination negotiate the drag operation privately.

static var move: NSDragOperation

A constant that indicates the drag can move the data.

static var delete: NSDragOperation

A constant that indicates the drag can delete the data.

static var every: NSDragOperation

A constant that indicates that drag can perform all of the drag operations.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

### Deprecated

static var all: NSDragOperation

Use every instead.

Deprecated

static var all_Obsolete: NSDragOperation

The `NSDragOperationAll` constant is deprecated. Use every instead.

Deprecated

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

struct NSDraggingItemEnumerationOptions

A group of constants that specify options to use when enumerating dragging items.

enum NSSpringLoadingHighlight

A group of constants that indicate a highlighting style for your app’s user interface to display during a spring-loading operation.

enum NSDraggingFormation

Constants that control the visual format of multiple dragging items.

enum NSDraggingContext

Constants that specify whether a drag terminates within or outside the application.

