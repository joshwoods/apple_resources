

- AVFAudio
- Audio Engine
-  Audio Units 

API Collection

# Audio Units

The data type for a plug-in component that provides audio processing or audio data generation.

## Topics

### Essentials

Creating an audio unit extension

Build an extension by using an Xcode template.

Using voice processing

Add voice-processing capabilities to your app by using audio engine.

class AVAudioUnit

A subclass of the audio node class that, processes audio either in real time or nonreal time, depending on the type of the audio unit.

### Component management

class AVAudioUnitComponent

An object that provides details about an audio unit.

class AVAudioUnitComponentManager

An object that provides a way to search and query audio components that the system registers.

### Audio effects

class AVAudioUnitEffect

An object that processes audio in real time.

class AVAudioUnitEQ

An object that implements a multiband equalizer.

class AVAudioUnitDistortion

An object that implements a multistage distortion effect.

class AVAudioUnitDelay

An object that implements a delay effect.

class AVAudioUnitReverb

An object that implements a reverb effect.

### Time effects

class AVAudioUnitTimeEffect

An object that processes audio in nonreal time.

class AVAudioUnitTimePitch

An object that provides a good-quality playback rate and pitch shifting independently of each other.

class AVAudioUnitVarispeed

An object that allows control of the playback rate.

### Audio generation

class AVAudioUnitGenerator

An object that generates audio output.

### Speech synthesis

Creating a custom speech synthesizer

Use your custom voices to synthesize speech by building a speech synthesis provider.

class AVSpeechSynthesisProviderAudioUnit

An object that generates speech from text.

### MIDI

class AVAudioUnitMIDIInstrument

An object that represents music devices or remote instruments.

## See Also

### Effects

Creating custom audio effects

Add custom audio-effect processing to apps like Logic Pro X and GarageBand by creating Audio Unit (AU) plug-ins.

