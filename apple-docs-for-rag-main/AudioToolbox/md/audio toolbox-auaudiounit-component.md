

- Audio Toolbox
- AUAudioUnit
-  component 

Instance Property

# component

The component found in the component description with which the audio unit was created.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var component: AudioComponent { get }
```

## See Also

### Describing the Audio Unit

var componentDescription: AudioComponentDescription

The component description with which the audio unit was created.

var componentName: String?

The audio unit’s component’s name.

var componentVersion: UInt32

The audio unit’s component’s version.

var audioUnitName: String?

The audio unit’s name, derived from the component’s name.

var audioUnitShortName: String?

var manufacturerName: String?

The manufacturer’s name, derived from the component’s name.

