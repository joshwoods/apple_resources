

- AVKit
- AVCaptureEventInteraction
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether this capture event interaction is in an enabled state.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

Set this value to false when your app can’t or won’t respond to the action callbacks to avoid non-interactive buttons or UI elements.

