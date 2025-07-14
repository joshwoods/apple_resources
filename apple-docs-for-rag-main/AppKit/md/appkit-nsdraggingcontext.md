

- AppKit
-  NSDraggingContext 

Enumeration

# NSDraggingContext

Constants that specify whether a drag terminates within or outside the application.

macOS 10.7+

``` source
enum NSDraggingContext
```

## Topics

### Constants

case outsideApplication

A constant that indicates dragging terminates outside the application.

case withinApplication

A constant that indicates dragging terminates within the application.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct NSDragOperation

A group of constants that represent which operations the dragging source can perform on dragging items.

struct NSDraggingItemEnumerationOptions

A group of constants that specify options to use when enumerating dragging items.

enum NSSpringLoadingHighlight

A group of constants that indicate a highlighting style for your app’s user interface to display during a spring-loading operation.

enum NSDraggingFormation

Constants that control the visual format of multiple dragging items.

