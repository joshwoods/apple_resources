

- AVFAudio
-  AVAudioEnvironmentDistanceAttenuationModel 

Enumeration

# AVAudioEnvironmentDistanceAttenuationModel

Types of distance attenuation models.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum AVAudioEnvironmentDistanceAttenuationModel
```

## Overview

Distance attenuation is the natural attenuation of sound when traveling from the source to the listener. The different attenuation models describe the drop-off in gain as the source moves away from the listener.

## Topics

### Attenuation Models

case exponential

An exponential model that describes the drop-off in gain as the source moves away from the listener.

case inverse

An inverse model that describes the drop-off in gain as the source moves away from the listener.

case linear

A linear model that describes the drop-off in gain as the source moves away from the listener.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting and Setting the Attenuation Model

var distanceAttenuationModel: AVAudioEnvironmentDistanceAttenuationModel

The distance attenuation model that describes the drop-off in gain as the source moves away from the listener.

