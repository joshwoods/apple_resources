

- Dispatch
- DispatchSource
-  DispatchSource.TimerFlags 

Structure

# DispatchSource.TimerFlags

Flags to use when configuring a timer dispatch source.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct TimerFlags
```

## Topics

### Timer Flags

static let strict: DispatchSource.TimerFlags

The system makes its best effort to observe the timer’s specified leeway value, even if the value is smaller than the default leeway.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating a Timer Source

class func makeTimerSource(flags: DispatchSource.TimerFlags, queue: DispatchQueue?) -> any DispatchSourceTimer

Creates a new dispatch source object for monitoring timer events.

protocol DispatchSourceTimer

A dispatch source that submits the event handler block based on a timer.

