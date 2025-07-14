

- AppKit
-  NSDraggingFormation 

Enumeration

# NSDraggingFormation

Constants that control the visual format of multiple dragging items.

macOS 10.7+

``` source
enum NSDraggingFormation
```

## Topics

### Constants

case `default`

A constant that represents the system determined formation.

case none

A constant that represents no custom formation, so drag images maintain their set positions relative to each other.

case pile

A constant that represents a pile formation, so drag images display on top of each other with random rotations.

case list

A constant that represents a list formation, so drag images display vertically, non-overlapping with the left edges aligned.

case stack

A constant that represents a stack formation, so drag images display overlapping diagonally.

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

enum NSDraggingContext

Constants that specify whether a drag terminates within or outside the application.

