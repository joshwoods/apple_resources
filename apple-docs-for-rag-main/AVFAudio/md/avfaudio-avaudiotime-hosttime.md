

- AVFAudio
- AVAudioTime
-  hostTime 

Instance Property

# hostTime

The host time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hostTime: UInt64 { get }
```

## See Also

### Manipulating Host Time

var isHostTimeValid: Bool

A Boolean value that indicates whether the host time value is valid.

class func hostTime(forSeconds: TimeInterval) -> UInt64

Converts seconds to host time.

class func seconds(forHostTime: UInt64) -> TimeInterval

Converts host time to seconds.

