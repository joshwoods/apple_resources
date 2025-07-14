

- Accessibility
-  AXLiveAudioGraph 

Class

# AXLiveAudioGraph

An object that represents an audio graph for a live-updating, continuous data series for VoiceOver.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AXLiveAudioGraph
```

## Overview

Use AXLiveAudioGraph to interact with an ongoing, continuous stream of data that updates with new data in real time.

## Topics

### Controlling playback

class func start()

Begins the live audio graph session.

class func stop()

Ends the live audio graph session.

### Configuring pitch

class func updateValue(Double)

Sets the pitch of the audio graph’s tone.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

