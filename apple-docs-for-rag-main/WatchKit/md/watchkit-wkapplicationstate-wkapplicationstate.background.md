

- WatchKit
- WKApplicationState
-  WKApplicationState.background 

Case

# WKApplicationState.background

The Watch app is running in the background.

watchOS 3.0+

``` source
case background
```

## Mentioned in 

Handling Common State Transitions

Working with the watchOS app life cycle

## Discussion

The system can wake suspended apps in the background. It can also launch apps that are not running in the background to perform background tasks.

## See Also

### Constants

case active

The Watch app is running in the foreground and currently receiving events.

case inactive

The Watch app is running in the foreground, but is not yet responding to actions from controls or gestures.

