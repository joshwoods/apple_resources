

- AppKit
- NSPageController
-  NSPageController.TransitionStyle 

Enumeration

# NSPageController.TransitionStyle

These constants control the transition style of the page controller.

macOS 10.8+

``` source
enum TransitionStyle
```

## Overview

These transition styles are independent of the delegate’s specification of book or history mode. It is perfectly reasonable to create a history style user interface using the book mode delegate methods. Simply set the transition style appropriately.

## Topics

### Constants

case stackHistory

Pages are stacked on top of each other. Pages animate out to the right to reveal the previous page. Next pages animate in from the right.

case stackBook

Pages are stacked on top of each other. Pages animate out to the left to reveal the next page. Previous pages animate in from the left.

case horizontalStrip

Each page is laid out next to each other in one long horizontal strip

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

