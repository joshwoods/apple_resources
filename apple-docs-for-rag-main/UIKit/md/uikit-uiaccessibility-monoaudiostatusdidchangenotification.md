

- UIKit
- UIAccessibility
-  monoAudioStatusDidChangeNotification 

Type Property

# monoAudioStatusDidChangeNotification

A notification that UIKit posts when system audio changes from stereo to mono.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let monoAudioStatusDidChangeNotification: NSNotification.Name
```

## Discussion

This notification doesn’t include a parameter. Observe this notification using the default notification center.

## See Also

### Audio and speech

static let speakScreenStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Screen setting changes.

static let speakSelectionStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Selection setting changes.

static let hearingDevicePairedEarDidChangeNotification: NSNotification.Name

A notification that UIKit posts when there’s a change to the currently paired hearing devices.

