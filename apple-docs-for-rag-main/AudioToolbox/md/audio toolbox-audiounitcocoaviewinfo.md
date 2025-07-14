

- Audio Toolbox
-  AudioUnitCocoaViewInfo 

Structure

# AudioUnitCocoaViewInfo

The name and number of custom Cocoa views for an audio unit.

macOS

``` source
struct AudioUnitCocoaViewInfo
```

## Topics

### Initializers

init(mCocoaAUViewBundleLocation: Unmanaged&lt;CFURL>, mCocoaAUViewClass: Unmanaged&lt;CFString>)

### Instance Properties

var mCocoaAUViewBundleLocation: Unmanaged&lt;CFURL>

var mCocoaAUViewClass: Unmanaged&lt;CFString>

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Configuring the Audio Unit UI

func GetAudioUnitParameterDisplayType(AudioUnitParameterOptions) -> AudioUnitParameterOptions

func SetAudioUnitParameterDisplayType(AudioUnitParameterOptions, AudioUnitParameterOptions) -> AudioUnitParameterOptions

