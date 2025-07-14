

- Core Haptics
- CHHapticEvent
-  init(audioResourceID:parameters:relativeTime:duration:) 

Initializer

# init(audioResourceID:parameters:relativeTime:duration:)

Initializes a haptic event from a previously loaded audio resource, specifying event parameters, start time, and duration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(
    audioResourceID resID: CHHapticAudioResourceID,
    parameters eventParams: [CHHapticEventParameter],
    relativeTime time: TimeInterval,
    duration: TimeInterval
)
```

## Parameters 

`resID`  

The resource ID of the accompanying audio signal.

`eventParams`  

An array of event parameters to characterize the audio event.

`time`  

The start time of the audio event, in seconds.

`duration`  

The duration of the audio event, in seconds.

## Discussion

To register an audio resource, call the CHHapticEngine object’s registerAudioResource(_:options:) method.

## See Also

### Creating Haptic Events

init(audioResourceID: CHHapticAudioResourceID, parameters: [CHHapticEventParameter], relativeTime: TimeInterval)

Initializes a haptic event from a previously loaded audio resource, specifying event parameters and start time.

init(eventType: CHHapticEvent.EventType, parameters: [CHHapticEventParameter], relativeTime: TimeInterval)

Initializes a haptic event of the specified type, parameters, and start time.

init(eventType: CHHapticEvent.EventType, parameters: [CHHapticEventParameter], relativeTime: TimeInterval, duration: TimeInterval)

Initializes a haptic event of the specified type, parameters, start time, and duration.

