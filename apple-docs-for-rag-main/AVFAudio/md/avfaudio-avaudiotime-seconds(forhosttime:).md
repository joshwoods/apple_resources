

- AVFAudio
- AVAudioTime
-  seconds(forHostTime:) 

Type Method

# seconds(forHostTime:)

Converts host time to seconds.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func seconds(forHostTime hostTime: UInt64) -> TimeInterval
```

## Parameters 

`hostTime`  

The host time.

## Return Value

The number of seconds that represent the host time you specify.

## See Also

### Manipulating Host Time

var hostTime: UInt64

The host time.

var isHostTimeValid: Bool

A Boolean value that indicates whether the host time value is valid.

class func hostTime(forSeconds: TimeInterval) -> UInt64

Converts seconds to host time.

