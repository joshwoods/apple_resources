

- DockKit
- DockAccessory
-  DockAccessory.FramingMode 

Enumeration

# DockAccessory.FramingMode

The mode to control framing of the subject when tracking.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
enum FramingMode
```

## Overview

The default is DockAccessory.FramingMode.automatic, which works well for most situations. DockAccessory.FramingMode.center keeps the subject close to the middle of frame. Similarly, DockAccessory.FramingMode.left and DockAccessory.FramingMode.right aligns the subject close to the left and right third of the frame (left, center, right).

## Topics

### Defining the framing mode

case automatic

Automatically frame the subject.

case center

Frame the subject in the center of the frame.

case left

Frame the subject in the left side of the frame.

case right

Frame the subject in the right side of the frame.

### Operators

static func == (DockAccessory.FramingMode, DockAccessory.FramingMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Setting framing mode

func setFramingMode(DockAccessory.FramingMode) async throws

Customize the dock accessory’s tracking behavior.

var framingMode: DockAccessory.FramingMode

The current framing mode.

