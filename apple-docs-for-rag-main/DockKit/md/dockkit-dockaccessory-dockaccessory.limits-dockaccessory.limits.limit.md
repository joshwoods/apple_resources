

- DockKit
- DockAccessory
- DockAccessory.Limits
-  DockAccessory.Limits.Limit 

Structure

# DockAccessory.Limits.Limit

A description of a limit placed on an axis of rotation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Limit
```

## Overview

Zero is the default minimum angular speed. Invalid limit specifications include minimum position greater than maximum position, minimum position equals maximum position, and maximum speed is less than zero.

## Topics

### Limiting speed and position

let maximumSpeed: Double

The maximum speed that the dock accessory moves.

let positionRange: Range&lt;Double>

The valid range that the dock accessory moves.

### Initializers

init(positionRange: Range&lt;Double>, maximumSpeed: Double) throws

## Relationships

### Conforms To

- Sendable

