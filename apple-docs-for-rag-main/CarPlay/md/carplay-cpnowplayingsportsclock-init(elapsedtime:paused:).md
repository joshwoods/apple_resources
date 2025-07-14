

- CarPlay
- CPNowPlayingSportsClock
-  init(elapsedTime:paused:) 

Initializer

# init(elapsedTime:paused:)

Represents a duration of time that has elapsed so far in this event, or play period of the event (quarter/inning/period).

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+

``` source
init(
    elapsedTime: TimeInterval,
    paused: Bool
)
```

## Discussion

When displayed on the now playing screen, the clock will count UP.

