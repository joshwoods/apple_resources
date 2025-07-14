

- Core Media
- CMTimebase
-  setTimerNextFireTime(\_:fireTime:) 

Instance Method

# setTimerNextFireTime(\_:fireTime:)

Sets the time on the timebase’s timeline at which the timer should fire next.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setTimerNextFireTime(
    _ timer: Timer,
    fireTime: CMTime
) throws
```

## See Also

### Setting Timers

func setTimerNextFireTime&lt;T>(T, fireTime: CMTime) throws

Sets the time on the timebase’s timeline at which the timer dispatch source should fire next.

func setTimerToFireImmediately(Timer) throws

Sets the timer to fire immediately once, overriding any previous calls.

func setTimerToFireImmediately&lt;T>(T) throws

Sets the timer dispatch source to fire immediately once, overriding any previous calls.

