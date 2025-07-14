

- AppKit
-  NSDraggingItemEnumerationOptions 

Structure

# NSDraggingItemEnumerationOptions

A group of constants that specify options to use when enumerating dragging items.

macOS 10.7+

``` source
struct NSDraggingItemEnumerationOptions
```

## Topics

### Constants

static var concurrent: NSDraggingItemEnumerationOptions

A constant that indicates the enumeration processes dragging items concurrently.

static var clearNonenumeratedImages: NSDraggingItemEnumerationOptions

A constant that indicates the enumeration clears the image components provider for all dragging items that don’t meet the classes and search options criteria.

### Initializers

init(rawValue: UInt)

Creates a dragging enumeration option with the specified raw value.

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

struct NSDragOperation

A group of constants that represent which operations the dragging source can perform on dragging items.

enum NSSpringLoadingHighlight

A group of constants that indicate a highlighting style for your app’s user interface to display during a spring-loading operation.

enum NSDraggingFormation

Constants that control the visual format of multiple dragging items.

enum NSDraggingContext

Constants that specify whether a drag terminates within or outside the application.

