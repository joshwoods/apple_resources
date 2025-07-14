

- Core Media
- CMTimebase
-  setTimerToFireImmediately(\_:) 

Instance Method

# setTimerToFireImmediately(\_:)

Sets the timer dispatch source to fire immediately once, overriding any previous calls.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setTimerToFireImmediately(_ timer: T) throws where T : DispatchSourceTimer
```

## See Also

### Setting Timers

func setTimerNextFireTime(Timer, fireTime: CMTime) throws

Sets the time on the timebase’s timeline at which the timer should fire next.

func setTimerNextFireTime&lt;T>(T, fireTime: CMTime) throws

Sets the time on the timebase’s timeline at which the timer dispatch source should fire next.

func setTimerToFireImmediately(Timer) throws

Sets the timer to fire immediately once, overriding any previous calls.

