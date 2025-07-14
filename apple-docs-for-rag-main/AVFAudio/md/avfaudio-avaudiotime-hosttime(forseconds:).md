

- AVFAudio
- AVAudioTime
-  hostTime(forSeconds:) 

Type Method

# hostTime(forSeconds:)

Converts seconds to host time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func hostTime(forSeconds seconds: TimeInterval) -> UInt64
```

## Parameters 

`seconds`  

The number of seconds.

## Return Value

The host time that represents the seconds you specify.

## See Also

### Manipulating Host Time

var hostTime: UInt64

The host time.

var isHostTimeValid: Bool

A Boolean value that indicates whether the host time value is valid.

class func seconds(forHostTime: UInt64) -> TimeInterval

Converts host time to seconds.

