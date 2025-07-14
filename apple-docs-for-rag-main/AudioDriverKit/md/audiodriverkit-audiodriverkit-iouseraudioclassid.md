

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioClassID 

Enumeration

# IOUserAudioClassID

An identifier for the type of audio object.

DriverKit 21.0+

``` source
enum IOUserAudioClassID : uint32_t;
```

## Topics

### General Objects

Object

The identifier for the audio object class.

### Device and Driver Objects

Device

The identifier for the audio device class.

Driver

The identifier for the audio driver class.

### Clock Objects

Clock

The identifier for the audio clock class.

### Container Obects

Box

The identifier for the audio box class.

### Stream Objects

Stream

The identifier for the audio stream class.

### General Controls

Control

The identifier for the audio control class.

### Slider Controls

SliderControl

The identifier for the audio slider control class.

### Level and Volume Control Objects

LevelControl

The identifier for the audio level control class.

VolumeControl

The identifier for the audio volume control class.

LFEVolumeControl

The identifier for the low-frequency effect volume control class.

### Boolean Controls

BooleanControl

The identifier for the audio Boolean control class.

LFEMuteControl

The identifier for the low-frequency effect mute control class.

SoloControl

The identifier for the audio solo control class.

JackControl

The identifier for the audio jack control class.

PhantomPowerControl

The identifier for the audio phantom power control class.

PhaseInvertControl

The identifier for the audio phase invert control class.

ClipLightControl

The identifier for the audio clip light control class.

TalkbackControl

The identifier for the audio talkback control class.

ListenbackControl

The identifier for the audio listenback control class.

### Mute Controls

MuteControl

The identifier for the audio mute control class.

### Selector Controls

SelectorControl

The identifier for the audio selector control class.

DataDestinationControl

The identifier for the audio data destination control class.

DataSourceControl

The identifier for the audio data source control class.

ClockSourceControl

The identifier for the audio clock source control class.

HighPassFilterControl

The identifier for the audio high pass filter control class.

LineLevelControl

The identifier for the audio line level control class.

### Channel Controls

StereoPanControl

The identifier for the stereo pan control class.

## See Also

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

