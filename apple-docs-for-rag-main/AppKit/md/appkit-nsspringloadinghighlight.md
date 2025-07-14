

- AppKit
-  NSSpringLoadingHighlight 

Enumeration

# NSSpringLoadingHighlight

A group of constants that indicate a highlighting style for your app’s user interface to display during a spring-loading operation.

macOS 10.11+

``` source
enum NSSpringLoadingHighlight
```

## Overview

The springLoadingHighlight method provides one of these constant values.

Do not use highlighting as a means to determine whether spring-loading has actually been activated or deactivated. The springLoadingActivated(_:draggingInfo:) method alerts your app when spring-loading activation occurs.

## Topics

### Constants

case none

A constant that indicates no highlighting.

case standard

A constant that indicates standard highlighting to show the destination supports spring-loading.

case emphasized

A constant that indicates emphasized highlighting to show active spring-loading on the destination.

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

enum NSDraggingFormation

Constants that control the visual format of multiple dragging items.

enum NSDraggingContext

Constants that specify whether a drag terminates within or outside the application.

