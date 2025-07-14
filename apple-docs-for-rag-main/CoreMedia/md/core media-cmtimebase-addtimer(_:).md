

- Core Media
- CMTimebase
-  addTimer(\_:) 

Instance Method

# addTimer(\_:)

Adds the timer dispatch source to the list of timers the timebase manages.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func addTimer(_ timer: T) throws where T : DispatchSourceTimer
```

## See Also

### Adding and Removing Timers

func addTimer(Timer, on: RunLoop) throws

Adds the timer to the list of timers the timebase manages.

func removeTimer(Timer) throws

Removes the timer from the list of timers the timebase manages.

func removeTimer&lt;T>(T) throws

Removes the timer dispatch source from the list of timers the timebase manages.

