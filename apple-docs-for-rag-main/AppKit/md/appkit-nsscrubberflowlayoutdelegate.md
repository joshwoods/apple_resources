

- AppKit
-  NSScrubberFlowLayoutDelegate 

Protocol

# NSScrubberFlowLayoutDelegate

A protocol that a scrubber delegate can adopt to provide the size of an item.

macOS

``` source
protocol NSScrubberFlowLayoutDelegate : NSScrubberDelegate
```

## Overview

This protocol conforms to the NSScrubberDelegate protocol. Create an object that conforms to NSScrubberFlowLayoutDelegate and assign it to the delegate property of your scrubber object.

## Topics

### Controlling the item size

func scrubber(NSScrubber, layout: NSScrubberFlowLayout, sizeForItemAt: Int) -> NSSize

Asks the delegate for the size of each item in a scrubber whose items are arranged in a flow layout.

## Relationships

### Inherits From

- NSObjectProtocol
- NSScrubberDelegate

## See Also

### Scrubber layouts

class NSScrubberFlowLayout

A concrete layout object that arranges items end-to-end in a linear strip.

class NSScrubberProportionalLayout

A concrete layout object that sizes each item to some fraction of the scrubber’s visible size.

class NSScrubberLayoutAttributes

The layout of a scrubber item.

class NSScrubberLayout

An abstract class that describes the layout of items within a scrubber control.

