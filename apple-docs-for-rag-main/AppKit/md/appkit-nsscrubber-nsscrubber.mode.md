

- AppKit
- NSScrubber
-  NSScrubber.Mode 

Enumeration

# NSScrubber.Mode

The scrolling behavior for a scrubber.

macOS 10.12.2+

``` source
enum Mode
```

## Overview

Scrolling is either *fixed* or *free*. For details on how to choose the correct scrolling mode for your app, see Choose a scrubber touch-interaction model.

## Topics

### Constants

case fixed

A scrolling mode in which scrubber items remain fixed in place, and the item under the user’s finger is highlighted.

case free

A scrolling mode in which the scrubber scrolls as the user swipes horizontally across the scrubber.

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

var itemAlignment: NSScrubber.Alignment

A setting that specifies the snapping behavior of items in the scrubber.

enum Alignment

The specified preferred alignment of items within the scrubber, when they come to rest following a user’s scrolling or paging interaction.

var isContinuous: Bool

A Boolean value that, together with the mode property, determines scrubber interaction style.

