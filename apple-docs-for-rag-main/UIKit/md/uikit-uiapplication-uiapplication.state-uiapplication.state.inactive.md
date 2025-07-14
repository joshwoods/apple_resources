

- UIKit
- UIApplication
- UIApplication.State
-  UIApplication.State.inactive 

Case

# UIApplication.State.inactive

The app is running in the foreground but isn’t receiving events.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
case inactive
```

## Discussion

This might happen as a result of an interruption or because the app is transitioning to or from the background.

## See Also

### Constants

case active

The app is running in the foreground and currently receiving events.

case background

The app is running in the background.

