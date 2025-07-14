

- AppKit
- NSScrubber
-  NSScrubber.Alignment 

Enumeration

# NSScrubber.Alignment

The specified preferred alignment of items within the scrubber, when they come to rest following a user’s scrolling or paging interaction.

macOS 10.12.2+

``` source
enum Alignment
```

## Overview

For details on how to choose the right alignment option for your app, see Choose a scrubber touch-interaction model.

## Topics

### Constants

case center

Center alignment of items within the scrubber.

case leading

Leading alignment of items within the scrubber.

case none

No preference for item alignment.

case trailing

Trailing alignment of items within the scrubber.

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

### Changing the layout

var scrubberLayout: NSScrubberLayout

An object used to describe the layout of items within the scrubber.

var mode: NSScrubber.Mode

A setting that determines whether interaction with the scrubber is fixed or free.

enum Mode

The scrolling behavior for a scrubber.

var itemAlignment: NSScrubber.Alignment

A setting that specifies the snapping behavior of items in the scrubber.

var isContinuous: Bool

A Boolean value that, together with the mode property, determines scrubber interaction style.

