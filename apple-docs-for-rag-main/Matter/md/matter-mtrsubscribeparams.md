

- Matter
-  MTRSubscribeParams 

Class

# MTRSubscribeParams

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRSubscribeParams
```

## Topics

### Initializers

init(minInterval: NSNumber, maxInterval: NSNumber)

### Instance Properties

var autoResubscribe: NSNumber?Deprecated

var keepPreviousSubscriptions: NSNumber?Deprecated

var maxInterval: NSNumber

var minInterval: NSNumber

var shouldReplaceExistingSubscriptions: Bool

var shouldReportEventsUrgently: Bool

var shouldResubscribeAutomatically: Bool

### Type Methods

class func new() -> SelfDeprecated

## Relationships

### Inherits From

- MTRReadParams

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

