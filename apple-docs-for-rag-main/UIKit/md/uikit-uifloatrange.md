

- UIKit
-  UIFloatRange 

Structure

# UIFloatRange

The range of motion for attached objects.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UIFloatRange
```

## Topics

### Creating a float range

init()

init(minimum: CGFloat, maximum: CGFloat)

Returns a new float range structure from the given components.

static let infinite: UIFloatRange

A range whose range is minus infinity to infinity.

static let zero: UIFloatRange

A range whose minimum and maximum are both `0.0`.

### Getting the range values

var maximum: CGFloat

The maximum range of motion for sliding and pin attachments.

var minimum: CGFloat

The minimum range of motion for sliding and pin attachments.

### Testing the range values

var isInfinite: Bool

Returns a Boolean indicating whether the specified float range is infinitely large.

func UIFloatRangeIsEqualToRange(UIFloatRange, UIFloatRange) -> Bool

Returns a Boolean indicating whether two float ranges are equivalent.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Constants

enum AttachmentType

Constants indicating the type of the attachment behavior object.

Float range constants

Constants for specifying standard ranges.

struct UIOffset

A structure that specifies an amount to offset a position.

