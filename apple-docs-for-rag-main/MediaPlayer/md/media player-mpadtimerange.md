

- Media Player
-  MPAdTimeRange 

Class

# MPAdTimeRange

An object that represents a time range where an ad break exists in the current player.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
class MPAdTimeRange
```

## Overview

This value must be in bounds of the duration of the current player item.

## Topics

### Creating an Ad Time Range

init(CMTimeRange)

Creates a Media Player time range that indicates where an ad break exists in the current player.

### Inspecting an Ad Time Range

var timeRange: CMTimeRange

A Media Player time range that indicates where an ad break exists in the current player.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

