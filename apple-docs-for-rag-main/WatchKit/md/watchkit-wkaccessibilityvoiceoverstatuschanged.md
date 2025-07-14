

- WatchKit
-  WKAccessibilityVoiceOverStatusChanged 

Global Variable

# WKAccessibilityVoiceOverStatusChanged

Tells the interface controller that the VoiceOver status has changed.

watchOS 2.0+

``` source
let WKAccessibilityVoiceOverStatusChanged: String
```

## Discussion

Use this notification to customize your application’s user interface for VoiceOver users. You can also use the isVoiceOverRunning function to determine whether VoiceOver is currently running.

Observe this notification using the default notification center. This notification doesn’t include a parameter.

