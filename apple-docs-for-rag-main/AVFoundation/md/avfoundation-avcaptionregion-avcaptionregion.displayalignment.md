

- AVFoundation
- AVCaptionRegion
-  AVCaptionRegion.DisplayAlignment 

Enumeration

# AVCaptionRegion.DisplayAlignment

Constants that indicate the alignment of lines in a region.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum DisplayAlignment
```

## Overview

When you insert a caption line, the region places it relative to existing lines. The system determines the order in which the region places lines by its block progression direction. For example, English captions’ block progression direction are top-to-bottom, while Japanese vertical captions use right-to-left.

## Topics

### Display Alignments

case before

An alignment that positions lines at the top of the block progression direction.

case center

An alignment that positions lines in the middle of the block progression direction.

case after

An alignment that positions lines at the bottom of the block progression direction.

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

### Accessing the Display Alignment

var displayAlignment: AVCaptionRegion.DisplayAlignment

The alignment of lines for the region.

