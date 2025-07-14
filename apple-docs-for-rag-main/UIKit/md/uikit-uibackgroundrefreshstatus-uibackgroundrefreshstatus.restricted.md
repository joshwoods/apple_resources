

- UIKit
- UIBackgroundRefreshStatus
-  UIBackgroundRefreshStatus.restricted 

Case

# UIBackgroundRefreshStatus.restricted

Background updates are unavailable and the user cannot enable them again.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
case restricted
```

## Discussion

For example, this status can occur when parental controls are in effect for the current user.

## See Also

### Constants

case denied

The user explicitly disabled background behavior for this app or for the whole system.

case available

Background updates are available for the app.

