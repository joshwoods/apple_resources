

- AVFoundation
- AVCaptureDeskViewApplication
- AVCaptureDeskViewApplication.LaunchConfiguration
-  requiresSetUpModeCompletion 

Instance Property

# requiresSetUpModeCompletion

A Boolean value that specifies whether the system requires the user to complete setup mode before it executes the completion handler.

Mac Catalyst 16.1+macOS 13.0+

``` source
var requiresSetUpModeCompletion: Bool { get set }
```

## Discussion

The default value is false, which tells the system to execute the completion handler as soon as it displays Desk View. If true, the system executes the completion handler after the user completes setup and starts Desk View.

## See Also

### Customizing the presentation

var mainWindowFrame: CGRect

The frame for Desk View after it launches.

