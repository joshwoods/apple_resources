

- SceneKit
-  SCNActionTimingMode 

Enumeration

# SCNActionTimingMode

Constants affecting the animation curve of an action, used by the timingMode property.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum SCNActionTimingMode
```

## Topics

### Constants

case linear

Linear pacing. The animation progresses evenly throughout its duration.

case easeIn

Ease-in pacing. The animation begins slowly, and then speeds up as it progresses.

case easeOut

Ease-out pacing. The animation begins quickly, and then slows as it completes.

case easeInEaseOut

Ease-in ease-out pacing. The animation begins slowly, accelerates through the middle of its duration, and then slows again before completing.

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

### Constants

typealias SCNActionTimingFunction

The signature for a block that manages animation timing, used by the timingFunction property.

