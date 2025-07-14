

- Foundation
- NSNotification
- NSNotification.Name
-  AVAudioUnitComponentTagsDidChange 

Type Property

# AVAudioUnitComponentTagsDidChange

A notification that indicates when component tags change.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
static let AVAudioUnitComponentTagsDidChange: NSNotification.Name
```

## Discussion

The notification object contains the `AVAudioUnitComponent` object with the tags.

## See Also

### AVFAudio

static let AVAudioEngineConfigurationChange: NSNotification.Name

A notification the framework posts when the audio engine configuration changes.

class let interruptionNotification: NSNotification.Name

A notification the system posts when an audio interruption occurs.

class let mediaServicesWereLostNotification: NSNotification.Name

A notification the system posts when it terminates the media server.

class let mediaServicesWereResetNotification: NSNotification.Name

A notification the system posts when the media server restarts.

class let routeChangeNotification: NSNotification.Name

A notification the system posts when its audio route changes.

class let silenceSecondaryAudioHintNotification: NSNotification.Name

A notification the system posts when the primary audio from other apps starts and stops.

