

- UIKit
- UIAccessibility
-  speakSelectionStatusDidChangeNotification 

Type Property

# speakSelectionStatusDidChangeNotification

A notification that UIKit posts when the system’s Speak Selection setting changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let speakSelectionStatusDidChangeNotification: NSNotification.Name
```

## Discussion

This notification doesn’t include a parameter. Observe this notification using the default notification center.

## See Also

### Audio and speech

static let monoAudioStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when system audio changes from stereo to mono.

static let speakScreenStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Screen setting changes.

static let hearingDevicePairedEarDidChangeNotification: NSNotification.Name

A notification that UIKit posts when there’s a change to the currently paired hearing devices.

