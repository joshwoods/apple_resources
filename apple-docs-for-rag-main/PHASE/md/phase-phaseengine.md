

- PHASE
-  PHASEEngine 

Class

# PHASEEngine

An object that manages audio assets, controls playback, and configures environmental effects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEEngine
```

## Overview

Before using PHASE, an app creates an instance of this object. Apps access all of the framework’s functionality through engine functions or properties, or through other PHASE classes into which you pass the engine object.

Important

You can create multiple engine instances, but normally, apps create only one.

### Create and Start the Engine

To create an engine object, choose a value for the init(updateMode:) argument that selects the desired control over scene setup and playback timing.

```
// Apps that need precise audio synchronization and 
// synchronized dynamic mix control pass in `.manual`.
engine = PHASEEngine(updateMode: .automatic) 
```

Then, load your sound assets, sound event assets, and shapes for sound occlusion. Before your app attempts to play sounds, start the engine object.

```
do { try engine.start() } 
catch { /* Handle the error. */ }
```

To stop audio playback and enable the engine to deallocate system resources, call the stop() function.

```
engine.stop()
```

## Topics

### Creating an Engine

init(updateMode: PHASEEngine.UpdateMode)

Creates an engine updated by the app or framework.

enum UpdateMode

Modes that determine when the framework consumes API calls and updates internal state.

### Registering Audio Resources

var assetRegistry: PHASEAssetRegistry

An object that loads and unloads audio resources.

### Accessing Scene Hierarchy

var rootObject: PHASEObject

The main object to which the app adds child objects.

### Defining Environmental Effects

var defaultReverbPreset: PHASEReverbPreset

The environmental surroundings that determine how sound resonates.

var defaultMedium: PHASEMedium

The physical matter through which sound travels.

var outputSpatializationMode: PHASESpatializationMode

The mode the engine implements to create a 3D sound experience.

### Controlling and Inspecting Playback State

func pause()

Pauses all audio playback.

func start() throws

Starts or resumes all audio playback.

func stop()

Stops all audio playback.

func update()

Processes app commands and increments framework processing.

var renderingState: PHASESoundEvent.RenderingState

The status of the engine’s audio playback.

### Managing Groups of Sounds

var groups: [String : PHASEGroup]

A list of named groups that contain sounds the app operates on collectively.

var activeGroupPreset: PHASEGroupPreset?

The settings that define playback for a group of sounds.

var duckers: [PHASEDucker]

An array of objects that reduce the volume of simultaneously playing sounds.

### Accessing In-Flight Audio

var soundEvents: [PHASESoundEvent]

A collection of the sounds that play under various runtime circumstances.

### Measuring Units

var unitsPerMeter: Double

A conversion factor from meters to your app’s preferred unit of measurement.

var unitsPerSecond: Double

A conversion factor from seconds to your app’s preferred unit of time.

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

## See Also

### Setup

enum UpdateMode

Modes that determine when the framework consumes API calls and updates internal state.

class PHASEAssetRegistry

A central repository of audio assets.

enum PHASENormalizationMode

Options that determine whether the framework adjusts a sound asset’s loudness for the user’s output device.

enum PHASESpatializationMode

The manner in which PHASE outputs spatial audio.

enum PHASEReverbPreset

The manner in which PHASE diffuses resonating sound.

class PHASEMedium

A property or quality of the environment that affects how sound travels.

