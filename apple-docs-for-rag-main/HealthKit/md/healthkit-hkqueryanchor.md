

- HealthKit
-  HKQueryAnchor 

Class

# HKQueryAnchor

An object used to identify all the samples previously returned by an anchored object query.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKQueryAnchor
```

## Overview

The system returns HKQueryAnchor objects in both the anchored object query’s results handler and it’s update handler. Use the anchors to query for samples added or deleted after the result or update.

## Topics

### Creating Anchor Objects

convenience init(fromValue: Int)

Returns an anchor object from the provided anchor value.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

