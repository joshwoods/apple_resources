

- Core Haptics
- CHHapticEvent
- CHHapticEvent.ParameterID
-  audioPan 

Type Property

# audioPan

The stereo panning of an audio event.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let audioPan: CHHapticEvent.ParameterID
```

## Discussion

This parameter value ranges from -1.0 (panned hard left) to 1.0 (panned hard right). The default value is 0.0 (center panned).

## See Also

### Audio Event Parameter IDs

static let audioVolume: CHHapticEvent.ParameterID

The volume of an audio event.

static let audioPitch: CHHapticEvent.ParameterID

The pitch of an audio event.

static let audioBrightness: CHHapticEvent.ParameterID

The high-frequency content of an audio event.

