

- SwiftUI
- LongPressGesture
-  init(minimumDuration:) 

Initializer

# init(minimumDuration:)

Creates a long-press gesture with a minimum duration

tvOS 14.0+

``` source
init(minimumDuration: Double = 0.5)
```

## Parameters 

`minimumDuration`  

The minimum duration of the long press that must elapse before the gesture succeeds.

## See Also

### Creating a long press gesture

init(minimumDuration: Double, maximumDistance: CGFloat)

Creates a long-press gesture with a minimum duration and a maximum distance that the interaction can move before the gesture fails.

var minimumDuration: Double

The minimum duration of the long press that must elapse before the gesture succeeds.

var maximumDistance: CGFloat

The maximum distance that the long press can move before the gesture fails.

