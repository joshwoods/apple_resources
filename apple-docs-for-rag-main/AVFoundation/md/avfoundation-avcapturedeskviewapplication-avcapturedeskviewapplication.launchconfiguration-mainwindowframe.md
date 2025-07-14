

- AVFoundation
- AVCaptureDeskViewApplication
- AVCaptureDeskViewApplication.LaunchConfiguration
-  mainWindowFrame 

Instance Property

# mainWindowFrame

The frame for Desk View after it launches.

Mac Catalyst 16.1+macOS 13.0+

``` source
var mainWindowFrame: CGRect { get set }
```

## Discussion

The default value is zero, which tells the system to use the previously set frame. The system uses global screen coordinates to display the frame. When Desk View launches from a native macOS app, the window origin is bottom-left. When it launches from a Mac Catalyst app, the window origin is top-left.

## See Also

### Customizing the presentation

var requiresSetUpModeCompletion: Bool

A Boolean value that specifies whether the system requires the user to complete setup mode before it executes the completion handler.

